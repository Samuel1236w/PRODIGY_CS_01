def caesar_cipher_encrypt(message, shift):
    encrypted_message = ""
    for char in message:
        if char.isalpha():  # Check if the character is a letter
            shift_base = 65 if char.isupper() else 97
            encrypted_message += chr((ord(char) - shift_base + shift) % 26 + shift_base)
        else:
            encrypted_message += char  # Keep non-alphabetic characters unchanged
    return encrypted_message

def caesar_cipher_decrypt(message, shift):
    return caesar_cipher_encrypt(message, -shift)

def main():
    print("Caesar Cipher Tool")
    while True:
        print("\nOptions:")
        print("1. Encrypt a message")
        print("2. Decrypt a message")
        print("3. Exit")
        choice = input("Enter your choice (1/2/3): ")

        if choice == "1":
            message = input("Enter the message to encrypt: ")
            shift = int(input("Enter the shift value: "))
            encrypted = caesar_cipher_encrypt(message, shift)
            print(f"Encrypted message: {encrypted}")
        elif choice == "2":
            message = input("Enter the message to decrypt: ")
            shift = int(input("Enter the shift value: "))
            decrypted = caesar_cipher_decrypt(message, shift)
            print(f"Decrypted message: {decrypted}")
        elif choice == "3":
            print("Exiting the program. Goodbye!")
            break
        else:
            print("Invalid choice. Please try again.")
if __name__ == "__main__":
    main()
