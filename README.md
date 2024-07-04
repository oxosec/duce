
# Discounted Udemy Course Enroller

![ViewCount](https://views.whatilearened.today/views/github/hoz-efa/Discounted-Udemy-Course-Enroller.svg)

Welcome to the Discounted Udemy Course Enroller project! This script helps you automatically enroll in free or discounted Udemy courses. It scrapes various websites offering Udemy course discounts and handles the enrollment process for you.

## Features

- **Automated Enrollment**: Automatically enrolls in free or discounted Udemy courses.
- **Multi-Account Support**: Supports multiple Udemy accounts for enrollment.
- **Customizable Settings**: Easily configurable settings for categories, languages, sites, and more.
- **Multiple Deployment Options**: Deployable using GitHub Actions, Koyeb, Heroku, or run locally.

## Running Locally

To run this script on your local device, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/hoz-efa/Discounted-Udemy-Course-Enroller.git
   cd Discounted-Udemy-Course-Enroller
   ```

2. **Install Dependencies**:
   Ensure you have Python installed. Then, install the required Python packages:
   ```bash
   pip install -r requirements.txt
   ```

3. **Configure Settings**:
   Edit the `duce-cli-settings.json` file to set your desired settings, or set the environment variables as described below.

4. **Run the Script**:
   ```bash
   python cli.py
   ```

## Configuring Settings

You can configure the settings either by modifying the `duce-cli-settings.json` file or by setting environment variables. The script prioritizes environment variables over the settings file.

### Environment Variables

Here are the environment variables you can set:

- `UDEMY_EMAIL`: Your Udemy email(s). For multiple accounts, separate emails with `|` (e.g., `email1|email2|email3`).
- `UDEMY_PASSWORD`: Your Udemy password(s). For multiple accounts, separate passwords with `|` (e.g., `password1|password2|password3`).
- `CATEGORIES_BUSINESS`: Set to `true` or `false`.
- `CATEGORIES_DESIGN`: Set to `true` or `false`.
- `CATEGORIES_DEVELOPMENT`: Set to `true` or `false`.
- `CATEGORIES_FINANCE_ACCOUNTING`: Set to `true` or `false`.
- `CATEGORIES_HEALTH_FITNESS`: Set to `true` or `false`.
- `CATEGORIES_IT_SOFTWARE`: Set to `true` or `false`.
- `CATEGORIES_LIFESTYLE`: Set to `true` or `false`.
- `CATEGORIES_MARKETING`: Set to `true` or `false`.
- `CATEGORIES_MUSIC`: Set to `true` or `false`.
- `CATEGORIES_OFFICE_PRODUCTIVITY`: Set to `true` or `false`.
- `CATEGORIES_PERSONAL_DEVELOPMENT`: Set to `true` or `false`.
- `CATEGORIES_PHOTOGRAPHY_VIDEO`: Set to `true` or `false`.
- `CATEGORIES_TEACHING_ACADEMICS`: Set to `true` or `false`.
- `LANGUAGES_ARABIC`: Set to `true` or `false`.
- `LANGUAGES_CHINESE`: Set to `true` or `false`.
- `LANGUAGES_DUTCH`: Set to `true` or `false`.
- `LANGUAGES_ENGLISH`: Set to `true` or `false`.
- `LANGUAGES_FRENCH`: Set to `true` or `false`.
- `LANGUAGES_GERMAN`: Set to `true` or `false`.
- `LANGUAGES_HINDI`: Set to `true` or `false`.
- `LANGUAGES_INDONESIAN`: Set to `true` or `false`.
- `LANGUAGES_ITALIAN`: Set to `true` or `false`.
- `LANGUAGES_JAPANESE`: Set to `true` or `false`.
- `LANGUAGES_KOREAN`: Set to `true` or `false`.
- `LANGUAGES_NEPALI`: Set to `true` or `false`.
- `LANGUAGES_POLISH`: Set to `true` or `false`.
- `LANGUAGES_PORTUGUESE`: Set to `true` or `false`.
- `LANGUAGES_ROMANIAN`: Set to `true` or `false`.
- `LANGUAGES_RUSSIAN`: Set to `true` or `false`.
- `LANGUAGES_SPANISH`: Set to `true` or `false`.
- `LANGUAGES_THAI`: Set to `true` or `false`.
- `LANGUAGES_TURKISH`: Set to `true` or `false`.
- `LANGUAGES_URDU`: Set to `true` or `false`.
- `SITES_DISCUDEMY`: Set to `true` or `false`.
- `SITES_UDEMY_FREEBIES`: Set to `true` or `false`.
- `SITES_TUTORIAL_BAR`: Set to `true` or `false`.
- `SITES_REAL_DISCOUNT`: Set to `true` or `false`.
- `SITES_COURSE_VANIA`: Set to `true` or `false`.
- `SITES_IDOWNLOADCOUPONS`: Set to `true` or `false`.
- `SITES_E_NEXT`: Set to `true` or `false`.
- `MIN_RATING`: Set a minimum rating (e.g., `4.5`).
- `SAVE_TXT`: Set to `true` or `false`.
- `DISCOUNTED_ONLY`: Set to `true` or `false`.

### Using GitHub Actions

You can automate the script to run every 24 hours using GitHub Actions. Here’s how:

1. **Fork the Repository**: First, fork the repository to your GitHub account.

2. **Set Secrets**: In your forked repository, go to `Settings` > `Secrets` > `Actions` and add the required secrets (e.g., `UDEMY_EMAIL`, `UDEMY_PASSWORD`).

3. **Workflow File**: The repository already contains a GitHub Actions workflow file. You can view and edit it here: [GitHub Actions Workflow](https://github.com/hoz-efa/Discounted-Udemy-Course-Enroller/blob/cli/.github/workflows/ci.yml).

   - This workflow runs the script every 24 hours.
   - It uses the secrets you set in the repository settings.

### Deployment on Koyeb or Heroku

If you prefer not to use GitHub Actions, you can deploy this script on platforms like Koyeb or Heroku.

#### Deploying on Koyeb

1. **Create a New Service**: Log in to Koyeb, create a new service, and connect your GitHub repository.
2. **Set Environment Variables**: Add the required environment variables in the service settings.

#### Deploying on Heroku

1. **Create a New Application**: Log in to Heroku, create a new application, and connect your GitHub repository.
2. **Set Environment Variables**: Go to the "Settings" tab and set the required environment variables in the Config Vars section.

By following these instructions, you can easily run and manage the Discounted Udemy Course Enroller script. Enjoy your free and discounted Udemy courses!
