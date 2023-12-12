
Algorithm: Is Palindrome
This algorithm determines if a word is a palindrome, meaning it reads the same from left to right and right to left.

Input: A word

Output: True if the word is a palindrome, False otherwise

Steps:

FUNCTION function_palindrome(word) : BOOLEAN
VAR
    word_length = len(word): INTEGER
BEGIN
    IF (word_length <= 1) THEN  // Base case: Empty word or single character is a palindrome
        RETURN  TRUE
        IF (if word[0] <> word[-1]) THEN //Different characters at ends, not a palindrome
            RETURN FALSE
        END_IF
    END_IF
    RETURN palindrome(word);
END
