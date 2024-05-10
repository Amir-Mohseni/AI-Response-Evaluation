# OlympiadQA

## Overview
OlympiadQA is a project designed to evaluate the performance of GPT-4 in solving Informatics Olympiad problems. The project provides a benchmarking platform where users can input Olympiad questions and compare GPT-4's generated answers to official solutions, aiming to assess the model's ability to tackle these complex challenges.

## Project Structure
- `evaluation_responses.csv`: Contains the evaluation results of GPT-4's responses to Olympiad questions.
- `QuestionSolver.ipynb`: Jupyter Notebook containing all the code for processing questions, generating answers, and evaluating responses.
- `requirements.txt`: File listing all the required libraries for running the notebook.

## Evaluation Format
The evaluations of GPT-4's responses follow a specific format, as demonstrated below:

Evaluation Response: 2.0
The model's response provides an incorrect solution. It breaks down the 8 points into 5 individual points and 1 combined point (representing the 3 collinear points), and then calculates combinations based on these 6 points, which is wrong. The proper solution would involve computing the combinations of the total 8 points and subtracting the combinations of the 3 collinear points (as they form 1 line), and then adding back that 1 line to account for the single line made up by the collinear points. The explanation and logic used by the model is flawed and does not provide the correct answer.


This format provides a detailed analysis of the model's response, including any flaws in logic and discrepancies from the correct solution.

## Usage
1. Clone the repository to your local machine.
2. Set your OpenAI API key as an environmental variable named `OPENAI_API_KEY`.
3. Open and run the `QuestionSolver.ipynb` notebook in a Jupyter environment.
4. Follow the instructions within the notebook to input Olympiad questions and evaluate GPT-4's responses.

## Contributing
Contributions to OlympiadQA are welcome! If you have ideas for improvements or would like to contribute to the project, feel free to submit pull requests or reach out to the project maintainers.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
