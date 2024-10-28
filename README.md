# TikTok Data Analysis

This repository contains a project analyzing a synthetic TikTok dataset. The dataset includes video transcriptions, user-generated comments, and various engagement metrics. The primary objective is to assist moderators in determining whether video content consists of unverified user claims or represents opinions on those claims.

## Project Structure

- **main_notebook.ipynb**: Contains the code for loading, exploring, and analyzing the dataset.

## Dataset

The dataset provides various metrics and properties of TikTok videos, including:
- Video metadata (ID, duration, views, likes, shares, etc.)
- Text transcriptions and author status
- Engagement metrics (comments, downloads)

### Data Dictionary

| Column name              | Type   | Description                                                                                             |
|--------------------------|--------|---------------------------------------------------------------------------------------------------------|
| `#`                      | int    | TikTok assigned number for video.                                                                       |
| `claim_status`           | obj    | Identifies if the video is a “claim” or an “opinion.”                                                   |
| `video_id`               | int    | Random identifier for the video.                                                                        |
| `video_duration_sec`     | int    | Video duration in seconds.                                                                              |
| `video_transcription_text` | obj | Transcribed text of the video.                                                                           |
| `verified_status`        | obj    | Indicates if the author is verified or not.                                                             |
| `author_ban_status`      | obj    | Shows if the author’s account is active, under scrutiny, or banned.                                     |
| `video_view_count`       | float  | View count of the video.                                                                                |
| `video_like_count`       | float  | Number of likes on the video.                                                                           |
| `video_share_count`      | float  | Number of shares.                                                                                       |
| `video_download_count`   | float  | Number of downloads.                                                                                    |
| `video_comment_count`    | float  | Number of comments on the video.                                                                        |

Source: [Coursera Dataset Project](https://www.coursera.org/learn/get-started-with-python/quiz/Ky5XE/activity-create-your-course-2-tiktok-project/attempt)

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/yourusername/repositoryname.git
   cd repositoryname
   ```

2. **Create a virtual environment** (recommended):
   ```bash
   python3 -m venv .venv
   source .venv/bin/activate
   ```

3. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Dataset**: Place your `tiktok_dataset.csv` in the root directory to load it successfully.

## Usage

1. **Data Loading**: The notebook demonstrates how to load and inspect the dataset.
2. **Exploratory Analysis**: It provides initial data inspection steps, handling null values, and exploring engagement metrics.
3. **Claim vs. Opinion Analysis**: Focuses on distinguishing user claims from opinions through transcription text analysis.
