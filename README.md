# CSC249
1.L.1 Git your feelings
Good morning everybody My favorite sport would be Volley Ball. Because it seems very fun and you get to be in a team jumping hitting a ball lol, But I also like seeing  teams having a bond and having one another back. And togetherness. And I always wanted to play but o have asthma so it sucked for me. 


#Brief description- Data structures
# Hello Data structures 
#CSC-249
#Winston Latoya

# Detective's list of suspects
suspects = ["John", "Jane", "Alex", "Morgan"]

# You are now investigating these suspects
print("Investigating the following suspects:")
for suspect in suspects:
    print(suspect)
    suspect_info = {
    "Norris": {"Alibi": "At the bar", "Motive": "Money"},
    "Latoya": {"Alibi": "At home", "Motive": "Revenge"},
    "Bob": {"Alibi": "In the office", "Motive": "Jealousy"}
}

# Investigating John's alibi
print("\nChecking norris alibi:")
print(suspect_info["Norris"]["Alibi"])

from collections import deque

# Queue of suspects in line for questioning
queue = deque(["Norris", "Latoya", "bob", "Morgan"])

# Question the first suspect in line
print("\nFirst suspect in line for questioning:")
first_suspect = queue.popleft()  # Get the first suspect
print(f"Interrogating {first_suspect}")

# Now the next suspect is up
print("\nNext in line for questioning:")
print(queue[0])

# Detective's set of evidence (no duplicates)
evidence = set()

# Add evidence pieces (without duplicates)
evidence.add("Fingerprints")
evidence.add("Footprints")
evidence.add("Witness Statement")
evidence.add("Fingerprints")  # Duplicate, won't be added

print("\nCollected evidence (no duplicates):")
for item in evidence:
    print(item)
    
    clue_stack = []

# Add some clues
clue_stack.append("Clue 1: Old note found at the crime scene")
clue_stack.append("Clue 2: Mysterious phone number")
clue_stack.append("Clue 3: Suspicious footprints")

# You're deep in the investigation, but you need to backtrack
print("\nBacktracking to the most recent clue:")
print(clue_stack.pop())  # Last clue added

# Check the next clue
print("\nNext clue to investigate:")
print(clue_stack[-1])
