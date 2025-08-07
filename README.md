# ICY_MCP

ICY_MCP is a toolkit for analyzing Instagram engagement using the Instagram Private API (unofficial). It provides a set of tools for post comment analysis, account engagement comparison, demographic extraction, lead identification, and engagement reporting.

> **Note:**  
> This server uses the Instagram Private API, which is not officially supported by Instagram. Use responsibly and in accordance with Instagram's terms of service. Be aware of rate limits to avoid being blocked by Instagram.

## Features

- **analyze_post_comments:** Analyze sentiment, themes, and potential leads from Instagram post comments.
- **compare_accounts:** Compare engagement metrics across multiple Instagram accounts.
- **extract_demographics:** Extract demographic insights from engaged users based on posts or accounts.
- **identify_leads:** Find potential leads by analyzing engagement patterns.
- **generate_engagement_report:** Generate comprehensive engagement reports for Instagram accounts over a specified date range.

## Usage

Each tool is accessed via its respective API endpoint or CLI command. Example usage and parameters are as follows:

### 1. Analyze Post Comments

```bash
analyze_post_comments(postUrl, maxComments=100)
```
- `postUrl`: URL of the Instagram post to analyze (required)
- `maxComments`: Maximum number of comments to analyze (optional, default 100)

### 2. Compare Accounts

```bash
compare_accounts(accounts, metrics='all')
```
- `accounts`: List of Instagram account handles to compare (required)
- `metrics`: Metrics to compare (optional, default 'all')

### 3. Extract Demographics

```bash
extract_demographics(accountOrPostUrl, sampleSize=50)
```
- `accountOrPostUrl`: Instagram account handle or post URL (required)
- `sampleSize`: Number of users to sample for demographic analysis (optional, default 50)

### 4. Identify Leads

```bash
identify_leads(accountOrPostUrl, criteria)
```
- `accountOrPostUrl`: Instagram account handle or post URL (required)
- `criteria`: Criteria for identifying leads (optional)

### 5. Generate Engagement Report

```bash
generate_engagement_report(account, startDate, endDate)
```
- `account`: Instagram account handle (required)
- `startDate`: Start date for the report (YYYY-MM-DD, optional)
- `endDate`: End date for the report (YYYY-MM-DD, optional)

## Installation

> **Note:**  
> This project requires Python 3.x and may need additional dependencies for interacting with the Instagram Private API.

```bash
git clone https://github.com/GeekyRiolu/ICY_MCP.git
cd ICY_MCP
# Install dependencies
pip install -r requirements.txt
```

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

## License

This project is licensed under the [MIT License](LICENSE).

## Disclaimer

This server uses the Instagram Private API, which is not officially supported by Instagram. Use responsibly and in accordance with Instagram's terms of service. Be aware of rate limits to avoid being blocked by Instagram.
