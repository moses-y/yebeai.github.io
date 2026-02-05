# Moses Yebei

Personal portfolio & rate card — AI Engineer & Data Scientist based in Nairobi, Kenya.

**Live:** [mosesyebei.github.io](https://mosesyebei.github.io)

## Features

- **Modern Dark Theme** — Clean, minimal design with CSS Grid
- **Rate Card** — Consultation, AI/ML Development, Data Science pricing
- **Skills Showcase** — Python, ML, AI Agents, LLMs, Cloud, Full-Stack
- **Opportunities Section** — Full-time roles, academic programs, GPU scholarships
- **Auto-Updating Forks Feed** — Daily GitHub Action fetches recent forks with Unsplash images

## Tech Stack

```
HTML5 + CSS3 (vanilla, no frameworks)
JavaScript (ES6+)
GitHub Actions (daily automation)
GitHub Pages (hosting)
```

## Project Structure

```
├── index.html              # Main portfolio page
├── forks.json              # Auto-generated forks data
├── scripts/
│   └── update-forks.js     # Fetches forks from GitHub API
├── .github/
│   └── workflows/
│       └── update-forks.yml  # Daily cron job
├── Resume/
│   └── MOSES_YEBEI_Resume.pdf
└── assets/                 # Legacy assets (CSS, JS, images)
```

## Auto-Updating Forks Feed

The site automatically updates daily with your latest forked repositories:

1. **GitHub Action** runs at midnight UTC
2. Fetches your 12 most recent forks via GitHub API
3. Maps repo topics to relevant Unsplash images
4. Generates `forks.json` and commits to repo
5. Site renders cards from the JSON data

### Manual Trigger

```bash
gh workflow run update-forks.yml
```

## Local Development

```bash
# Clone
git clone https://github.com/moses-y/mosesyebei.github.io.git
cd mosesyebei.github.io

# Serve locally
python -m http.server 8888

# Generate forks.json manually
node scripts/update-forks.js
```

## Rate Card

| Service | Rate |
|---------|------|
| Consultation | $40/hr |
| AI/ML Development | $60/hr |
| Data Science | $50/hr |

## Contact

- Email: mosesyebei@gmail.com
- LinkedIn: [moses-yebei](https://linkedin.com/in/moses-yebei)
- GitHub: [moses-y](https://github.com/moses-y)
- Medium: [@mosesmyn](https://medium.com/@mosesmyn)

## License

MIT
