# Experiment 3 – Logging, Timeouts and Retries

## Course Details

- **Course Name:** Generative AI and AI Platform Engineering
- **Course Code:** 25CS2207E
- **Module:** Module I
- **Experiment:** 3
- **CO Mapping:** CO1

## Aim

To log every Large Language Model (LLM) call with information such as token usage, latency and estimated cost into MongoDB, and make the client more reliable by implementing timeouts, retries with exponential backoff for HTTP 429/5xx errors, and fail-fast handling for HTTP 4xx errors.

## Experiment Overview

This experiment demonstrates how to monitor LLM API calls and handle errors efficiently.

The implementation uses Python and the Gemini API, with MongoDB as the preferred logging destination. If MongoDB is not configured or unavailable, the experiment automatically uses a JSONL file for storing call records.

## Technologies Used

- Python
- Google Gemini API
- Google Colab
- MongoDB Atlas (optional)
- PyMongo
- Pandas
- JSON / JSONL

## Implementation

The experiment is divided into four steps:

### Step 1 – Five Logged LLM Calls

- Sends five prompts to the Gemini model.
- Records input tokens, output tokens and thinking tokens.
- Measures API response latency.
- Calculates the estimated API cost.
- Records the number of attempts and success status for each call.

### Step 2 – Retry Demonstration (HTTP 503)

- Uses a simulated provider that fails twice with HTTP 503.
- Implements exponential backoff before retrying.
- Demonstrates successful execution after the third attempt.

### Step 3 – Fail-Fast Demonstration (HTTP 400)

- Simulates an HTTP 400 error.
- Demonstrates that client errors are not retried.
- Stops after the first failed attempt.

### Step 4 – Inspect the Call Log

- Retrieves the recorded LLM calls.
- Displays token usage, latency, cost, attempts and success status.
- Saves a sample of the latest three call records as a JSON file.

## Key Concepts Learned

- LLM call logging and monitoring
- Token usage tracking
- Latency measurement
- Estimated API cost calculation
- Request timeouts
- Retry mechanisms
- Exponential backoff
- HTTP 4xx and 5xx error handling
- MongoDB-based logging
- JSONL-based fallback logging

## Generated Outputs

The experiment generates the following files inside the `results` directory:

- `calls.jsonl` – stores LLM call records when JSONL logging is used.
- `exp03_sample_call_log.json` – stores a sample of the latest three experiment records.
- `results.zip` – compressed archive of the generated results.

The actual files generated depend on the logging configuration and successful execution.

## Execution

The notebook is executed in Google Colab by running all cells in sequence.

Required configuration:
- `GEMINI_API_KEY` – required for Gemini API calls.
- `MONGODB_URI` – optional; required for MongoDB logging.

## Repository Contents

- `Exp03_Logging_Timeouts_Retries.ipynb` – experiment implementation and execution outputs.
- `results.zip` – generated experiment results.
- `README.md` – experiment documentation.

## Conclusion

This experiment demonstrates how to monitor LLM API calls by recording token usage, latency and estimated cost. It also implements timeout and retry mechanisms to improve reliability, using exponential backoff for retryable server errors and fail-fast handling for client errors.
