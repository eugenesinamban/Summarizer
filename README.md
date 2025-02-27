# CLI Gmail Newsletter Summarizer

THIS IS STILL A WIP. WILL WORK ON THE FINER DETAILS LATER

This command-line tool automates the process of summarizing newsletter articles from your Gmail inbox and saving them as Markdown files in your Obsidian vault.

## Features

- Retrieves unread newsletter emails from Gmail.
- Extracts article links from email content.
- Summarizes articles using the Gemini API.
- Formats summaries as Obsidian-compatible Markdown (including YAML frontmatter).
- Saves summaries to a specified Obsidian vault directory.
- Supports configuration of API keys, vault paths, and sender email filters.
- Uses OAuth 2.0 for secure Gmail authentication.
- Securely stores tokens using the OS credential store.

## Installation

1. **Prerequisites:**
    - Go 1.18 or later.
    - A Google Cloud project with the Gmail API enabled.
    - A Gemini API key.
    - An Obsidian vault.
2. **Clone the Repository:**

    ```bash
    git clone [repository URL]
    cd [repository directory]
    ```

3. **Install Dependencies:**

    ```bash
    go mod tidy
    ```

4. **Build the Tool:**

    ```bash
    go build
    ```

## Configuration

1. **Gmail Authentication:**
    - Run `newsletter-summarizer auth` to initiate the OAuth 2.0 flow.
2. **Configuration Settings:**
    - Use the `newsletter-summarizer config` command to set your API key, Obsidian vault path, and sender email filters.
    - Example: `newsletter-summarizer config --api-key="your_gemini_api_key" --vault-path="/path/to/your/obsidian/vault" --sender="newsletter@example.com"`
3. **View Configuration:**
    - Use the `newsletter-summarizer view-config` command to view the current settings.

## Usage

- Run `newsletter-summarizer summarize` to retrieve, summarize, and save your newsletter articles.

## Contributing

Contributions are welcome! Please feel free to submit pull requests or open issues to report bugs or suggest new features.

## License

[Your License]

## Contact

eugene.sinamban@gmail.com
