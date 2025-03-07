# Function to reverse a string using string slicing
def reverse_with_slicing(s):
    return s[::-1]

# Function to reverse a string using loops and iteration
def reverse_with_loop(s):
    reversed_str = ""
    for char in s:
        reversed_str = char + reversed_str
    return reversed_str

# Main function to test both methods
def main():
    test_strings = ["hello", "Python", "OpenAI", "12345"]

    print("Reversing strings using String Slicing:")
    for string in test_strings:
        print(f"Original: {string} -> Reversed: {reverse_with_slicing(string)}")

    print("\nReversing strings using Loops and Iteration:")
    for string in test_strings:
        print(f"Original: {string} -> Reversed: {reverse_with_loop(string)}")

# Run the program
main()
