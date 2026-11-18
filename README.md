# Mood-sense
# Happy or Sad Sentence Predictor

sentence = input("Enter a sentence: ")

happy_words = ["happy", "joy", "great", "good", "excited", "love", "smile", "wonderful"]

sad_words = ["sad", "cry", "bad", "upset", "angry", "lonely", "pain", "sorry"]

sentence = sentence.lower()

happy_count = 0
sad_count = 0

for word in happy_words:
    if word in sentence:
        happy_count += 1

for word in sad_words:
    if word in sentence:
        sad_count += 1

if happy_count > sad_count:
    print("Result: Happy ")
elif sad_count > happy_count:
    print("Result: Sad ")
else:
    print("Result: Neutral ")

print("Thank you for using the program!")
