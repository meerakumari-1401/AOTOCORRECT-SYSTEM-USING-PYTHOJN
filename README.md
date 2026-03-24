from textblob import TextBlob

while True:
    text = input("\nEnter a sentence (type 'exit' to quit): ")

    if text.lower() == "exit":
        print("Program Ended")
        break

    blob = TextBlob(text)
    corrected = blob.correct()

    print("Corrected Sentence:", corrected).p
