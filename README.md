# pythonproject1
def main():
    questions = {
        "What is the capital of France?": "Paris",
        "What is 2 + 2?": "4",
        "What is the capital of Japan?": "Tokyo",
        "What is the chemical symbol for water?": "H2O",
        "Who wrote 'To Kill a Mockingbird'?": "Harper Lee"
    }

    score = 0

    for question, answer in questions.items():
        user_answer = input(question + " ")
        if user_answer.strip().lower() == answer.strip().lower():
            print("Correct!")
            score += 1
        else:
            print(f"Wrong! The correct answer is {answer}.")

    print(f"Your final score is {score} out of {len(questions)}.")

if __name__ == "__main__":
    main()
