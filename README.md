
def count_words(text):
    counts = {}

    for word in text.lower().split():
        counts[word] = counts.get(word, 0) + 1

    return counts


if __name__ == "__main__":
    sentence = (
        "practice makes progress and practice builds confidence"
    )

    print("Word frequencies:")
    for word, count in count_words(sentence).items():
        print(f"{word}: {count}")
