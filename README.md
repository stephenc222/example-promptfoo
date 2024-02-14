# Promptfoo Example

This example project uses the [Promptfoo](https://promptfoo.dev/docs/intro) tool to test a creative storytelling prompt testing various topics using a variety of Promptfoo assertions. It uses multiple AI providers such as Mistral and OpenAI's GPT models.

For a more thorough walkthrough, checkout the [companion blog post](https://stephencollins.tech/posts/how-to-use-promptfoo-for-llm-testing) that accompanies this example.

## Getting Started

1. Clone the repository to your local machine.

2. All you need to is a modern version of Node installed on your machine to run the Promptfoo CLI (through `npx` that comes bundled along with `npm` when installing Node) for this demo project.

3. Set your `OPENAI_API_KEY` and `MISTRAL_API_KEY` environment variables. You can do this by copying the `.env.example` file to a new file named `.env` and replacing the placeholder value with your actual OpenAI API and MISTRAL_API_KEY keys.

4. Edit the `promptfooconfig.yaml` file to customize the prompts, providers, and tests to explore Promptfoo as you wish!

## Running the Project

1. Run the test script `npm run test` to start the evaluation process.

2. After the evaluation is complete, you can view the test results in a local web UI by running `npm run view`.

3. To clear the Promptfoo test cache, you can run `npm run clean`.

4. For the sake of illustration, you should see 2 failures and 7 successes when running `npm run test`.

## Testing

The `promptfooconfig.yaml` file contains various tests that assert the cost, relevance, and other aspects of the generated content. These tests are run during the evaluation process.
