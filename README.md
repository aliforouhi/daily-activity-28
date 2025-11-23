# daily_update.p
import datetime
import random
import string

print("Daily GitHub activity - Day 28")

today = datetime.date.today()

# Generate a random password of length 10
characters = string.ascii_letters + string.digits
password = "".join(random.choice(characters) for _ in range(10))

# Count vowels in the password
vowels = "aeiouAEIOU"
vowel_count = sum(1 for char in password if char in vowels)

print(f"Today's date: {today}")
print(f"Generated password: {password}")
print(f"Number of vowels in password: {vowel_count}")
