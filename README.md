# fampay 
#youtube api fetching  kishan kumar newton school

Project Goal
To make an API to fetch latest videos sorted in reverse chronological order of the publishing date-time from YouTube for a given search query in paginated response

Basic Functionalities
Cron Job to constantly fetch data in the background every minute
GET API, /videos for fetching videos supporting options like sorting, fuzzy searching and pagination
Search API which also supports fuzzy matching for situations like How to make a tea? matched with tea how
Dashboard to access the videos with options to filter and search
Development


Clone the project


Copy .env.example to .env
# For default values, refer `.env.defaults` file
NODE_ENV = 

# Server Properties
PORT =

# MONGODB
MONGODB_URI = 

# YOUTUBE API
YOUTUBE_API_KEY =
YOUTUBE_SEARCH_QUERY =
You will need a YOUTUBE DATA API key in order to run this app. Follow the instructions on this page to get one.

Note:

For default values of environment variables, refer .env.defaults file
You will need to provide values to all those variables that do not have a default
Fields that don't have a default value are required
In case of multiple API keys, provide them as "," delimited list of keys like so:
YOUTUBE_API_KEY = "<API_KEY1>, <API_KEY2>..."
Install dependencies
npm install

Run in development mode
npm run dev

Running with Docker Compose
When using Docker Compose,

Create a .env file using the instructions mentioned above
Set the MONGODB_URI environment variable in your .env file to
MONGODB_URI = mongodb://mongo:27017
Run:
docker-compose up -d
Navigate to http://localhost:3000 to see the app live
Monitor the data dumped into MongoDB by navigating to http://localhost:8081 thanks to mongo-express
Resources
https://demos.creative-tim.com/argon-design-system/#/presentation
https://developers.google.com/youtube/v3
