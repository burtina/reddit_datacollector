# reddit_datacollector
Python-based Reddit discussion data collection and analysis tool

# Reddit Data Collector

## Project Overview

Reddit Data Collector is a Python-based application designed to collect and analyze publicly available Reddit posts and comments from selected communities related to dating apps and online dating experiences.

The project aims to organize Reddit discussions into structured datasets for analysis, including identifying common topics, user experiences, recurring concerns, and discussion patterns.

The application is currently in the planning stage, and Reddit Data API access is pending authorization.

## Project Objectives

- Collect publicly available posts and comments from selected Reddit communities.
- Extract relevant information such as post titles, text, scores, timestamps, and comment relationships.
- Organize collected information into structured CSV files.
- Analyze recurring themes and patterns in online dating discussions.
- Use Python-based data processing tools for analysis.

## Intended Subreddits

The proposed communities include:

- r/Tinder
- r/Bumble
- r/hingeapp
- r/OnlineDating
- r/dating_advice

The final selection will depend on Reddit API authorization, subreddit availability, and applicable community rules.

## Data Collection

The application is intended to collect the following fields, subject to Reddit's API permissions.

### Post Data

| Field | Description |
|---|---|
| Post ID | Unique identifier for a Reddit post |
| Title | Title of the post |
| Body | Text content of the post |
| Score | Reddit post score |
| Timestamp | Date and time the post was created |
| Subreddit | Community where the post was published |
| Number of Comments | Number of comments associated with the post |

### Comment Data

| Field | Description |
|---|---|
| Comment ID | Unique identifier for a comment |
| Comment Body | Text content of the comment |
| Score | Reddit comment score |
| Timestamp | Date and time the comment was created |
| Parent ID | Identifier of the parent post or comment |
| Post ID | Identifier of the associated post |

## Proposed Technical Stack

- **Programming Language:** Python
- **API:** Reddit Data API (subject to approval)
- **API Client:** PRAW (Python Reddit API Wrapper)
- **Data Processing:** pandas
- **Data Storage:** CSV files
- **Development Environment:** Visual Studio Code
- **Version Control:** Git and GitHub

## Proposed Application Workflow

1. Authenticate with Reddit using authorized OAuth credentials.
2. Retrieve permitted public posts from selected subreddits.
3. Retrieve comments associated with those posts.
4. Extract the required data fields.
5. Organize the records using Python and pandas.
6. Export the processed data to CSV files for analysis.

## Why an External Python Application?

The project requires an external Python environment for data collection, processing, and analysis.

The proposed workflow uses Python libraries such as pandas to organize and transform records into structured datasets. It is intended to run independently of Reddit's Devvit application environment.

## Privacy and API Compliance

The application is intended to operate in read-only mode and will not automatically post, comment, vote, or send messages.

The project will:

- Access only data permitted by Reddit's API and applicable policies.
- Respect API rate limits and authorization requirements.
- Avoid collecting private messages or accessing private communities without authorization.
- Avoid publishing API credentials or authentication tokens.
- Apply appropriate safeguards to stored data.
- Follow applicable requirements concerning data retention, deletion, and permitted use.

The application will not begin API data collection until the necessary authorization has been obtained.

## Development Status

**Status: Planning — API authorization not yet obtained.**

Planned development stages:

1. Prepare project documentation and repository.
2. Obtain Reddit Data API authorization.
3. Configure the Python development environment.
4. Implement API authentication.
5. Develop post and comment collection functionality.
6. Export permitted data to CSV files.
7. Perform data analysis and evaluate the results.

## Intended Outcome

The expected outcome is a structured dataset of permitted Reddit discussions that can support analysis of recurring themes, user experiences, and concerns related to dating applications.

The project is intended for read-only data collection and analysis, subject to Reddit's authorization and developer policies.
