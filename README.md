
def calculate_average_word_length(text):
    words = text.split()

    if not words:
        return 0

    total_length = sum(len(word) for word in words)
    return round(total_length / len(words), 2)


if __name__ == "__main__":
    sentence = "Consistency and patience create long term success"

    print(f"Sentence: {sentence}")
    print(
        f"Average word length: "
        f"{calculate_average_word_length(sentence)}"
    )
