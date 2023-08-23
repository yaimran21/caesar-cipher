from art import logo
alphabet = ['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z']


def caesar(start_text, shift_amount, cipher_direction):
    cipher_text = ""
    if cipher_direction == "decode":
        shift_amount *= -1
    # print(direction + " " + str(shift) + " " + text)
    for letter in start_text:
        if letter in alphabet:
            position = alphabet.index(letter)
            position = position + shift_amount
            cipher_text += alphabet[position]
        else:
            cipher_text += letter
    print(f"The {direction}d text is: {cipher_text}")


print(logo)

should_continue = True
while should_continue:
    direction = input("Type 'encode' to encrypt, type 'decode' to decrypt:\n").lower()
    text = input("Type your message:\n").lower().replace(" ", "")
    shift = int(input("Type the shift number:\n"))
    shift = shift % 26
    caesar(start_text=text, shift_amount=shift, cipher_direction=direction)
    result = input("If you want to continue type 'yes' otherwise type 'no'\n ").lower()

    if result == 'no':
        should_continue = False
        print("Goodbye")
