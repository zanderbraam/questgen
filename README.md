# QuestGen

**QuestGen** is a Streamlit app designed to generate custom question sets aimed at developing instruments for measuring the communicative participation outcomes of school-aged children (6 to 11 years old) with communication difficulties. This tool assists speech-language therapists (SLTs) and parents in assessing and understanding children's participation in social contexts where communication is essential.

## Features

- **Dynamic Question Generation**: Create sets of 10 questions tailored to specific communicative participation scenarios.
- **User-Friendly Interface**: Utilize dropdown menus to select options and generate questions effortlessly.
- **Customizable Focus Areas**: Choose from various aspects of communication, such as verbal skills, non-verbal cues, social interaction, and understanding.

## Purpose

The aim of QuestGen is to support the development of assessment instruments that measure how children with communication difficulties engage in life situations involving the exchange of knowledge, information, ideas, and feelings. By providing relevant and targeted questions, the app helps SLTs and parents evaluate and enhance the communicative participation of children in social and educational settings.

## Getting Started

Follow these steps to set up and run QuestGen on your local machine.

### Prerequisites

- **Python 3.11**
- **virtualenv** installed
- **Git** installed

### Installation

1. **Clone the Repository**:

   ```bash
   git clone https://github.com/zanderbraam/questgen.git
   ```

2. **Navigate to the Project Directory**:

   ```bash
   cd questgen
   ```

3. **Create a Virtual Environment**:

   Using `virtualenv` with Python 3.11:

   ```bash
   virtualenv ve -p /usr/bin/python3.11
   ```

4. **Activate the Virtual Environment**:

   - On Linux/MacOS:

     ```bash
     source ve/bin/activate
     ```

   - On Windows:

     ```bash
     ve\Scripts\activate
     ```

5. **Upgrade `pip` to Version 24.3.1**:

   ```bash
   pip install --upgrade pip==24.3.1
   ```

6. **Install Dependencies**:

   ```bash
   pip install -r requirements.txt
   ```

### Local Testing

To run the app locally, you need to provide your OpenAI API key. Follow these steps:

1. **Set Up Environment Variables**:

   Create a `.env` file in the root directory of the project to securely store your OpenAI API key.

   ```bash
   touch .env
   ```

   Add the following line to your `.env` file:

   ```env
   OPENAI_API_KEY=your_openai_api_key_here
   ```

   Replace `your_openai_api_key_here` with your actual OpenAI API key.

   > **Note:** Ensure that your `.env` file is included in your `.gitignore` to prevent it from being committed to version control.

2. **Run the App**:

   ```bash
   streamlit run app.py
   ```

3. **Using the App Locally**:

   - **Select Options**: Use the dropdown menu to choose specific communication aspects you wish to focus on.
   - **Generate Questions**: Click the 'Generate' button to produce a set of 10 tailored questions.
   - **Review and Utilize**: Use the generated questions for assessment, therapy planning, or research purposes.

### Using the Deployed Version

You can access the deployed version of QuestGen using the following link:

[Access QuestGen Online](https://your-deployed-app-link.com)

*Note: Replace the above link with the actual URL after deployment.*

## Contributing

Contributions are welcome! Please open an issue or submit a pull request for any improvements or suggestions.

## License

This project is licensed under the [MIT License](LICENSE).