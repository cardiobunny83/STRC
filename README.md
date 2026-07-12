# STRC
What This Code Actually Does
The Big Picture
Think of this like building a YouTube-like website specifically for your organization's videos, chapel services, and documents. It has two main areas:

Part 1: The Chapel Section (The "Chapel Access" Area)
What it looks like to users:

A prominent, colorful section at the top of your website
Shows the latest chapel service with a big video player
If there's a live service happening right now, it shows a red "LIVE NOW" banner
Has two buttons: "Watch Now" (for video) and "Listen Now" (for audio/podcast version)
A link to browse all past chapel services
What happens behind the scenes:

Automatically pulls the most recent chapel recording
Detects if a live stream is active
Keeps track of how many people watch each video
Stores information like who spoke, what scripture was read, and when it happened
Part 2: The Archive Section (The "Archive Access" Area)
What it looks like to users:

A search bar where people can type keywords (like a speaker's name, topic, or Bible verse)
Category buttons to filter: "Chapel Services," "Past Events," "Trainings," or "Newsletters"
Date filters to find content from specific time periods
A grid of results showing thumbnails, titles, and quick info
Each item has action buttons: "Watch," "Listen," or "Read"
What happens behind the scenes:

When someone searches, it quickly scans through:
Video titles and descriptions
Full transcripts of what's said in the videos
Speaker names
Tags and categories
Returns results ranked by relevance
Tracks what people watch and what's popular
The "Brains" of the System (The Database)
Think of this like a super-organized filing cabinet:

PostgreSQL (The Main Filing Cabinet):

Stores all the basic info: titles, dates, speakers, video URLs
Organizes content into categories
Keeps track of view counts and what's featured
MongoDB (The Document Storage):

Stores longer content like full video transcripts
Saves "chapters" (timestamps for different parts of a video)
Tracks user engagement (comments, bookmarks)
Elasticsearch (The Search Engine):

Like Google for your content
Makes searching instant, even with thousands of videos
Can find words inside video transcripts
The Video Player
Plays videos directly in the browser (no download needed)
Works with modern streaming technology (like Netflix uses)
Shows a progress bar you can click to jump around
Works on phones, tablets, and computers
