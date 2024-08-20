
```markdown
# NFT Collection

This project demonstrates a simple implementation of an NFT (Non-Fungible Token) collection using JavaScript. It allows you to create NFTs with metadata, list them, and check the total supply of NFTs created.

## Project Structure

- `NFT` Class: A blueprint for creating NFT objects with metadata such as title, description, and image URL.
- `myNFTs` Array: A collection that holds all the NFTs created.
- `createNFT` Function: Creates a new NFT with the provided metadata and stores it in the `myNFTs` array.
- `listNFTs` Function: Iterates over the array of NFTs and prints their metadata to the console.
- `getTotalSupply` Function: Returns the total number of NFTs created.

## How to Use

1. **Create NFTs:**

   You can create NFTs by calling the `createNFT` function and passing the title, description, and image URL as arguments.

   ```javascript
   createNFT("C", "C Language", "https://example.com/image1.png");
   createNFT("Python", "Python Language", "https://example.com/image2.png");
   createNFT("Java", "Java Language", "https://example.com/image3.png");
   createNFT("JS", "Java Script", "https://example.com/image4.png");
   ```

2. **List NFTs:**

   To view all the NFTs you have created, call the `listNFTs` function. It will print the title, description, and image URL of each NFT to the console.

   ```javascript
   console.log("Listing NFTs:");
   listNFTs();
   ```

3. **Get Total Supply:**

   To find out how many NFTs have been created, call the `getTotalSupply` function. It will return the total count.

   ```javascript
   console.log("Total NFTs created: " + getTotalSupply());
   ```

## Example Output

```javascript
Listing NFTs:
Title: C
Description: C Language
Image URL: https://example.com/image1.png
----------------------
Title: Python
Description: Python Language
Image URL: https://example.com/image2.png
----------------------
Title: Java
Description: Java Language
Image URL: https://example.com/image3.png
----------------------
Title: JS
Description: Java Script
Image URL: https://example.com/image4.png
----------------------
Total NFTs created: 4
```

## Technologies Used

- JavaScript

## License

This project is open source and available under the [MIT License](https://opensource.org/licenses/MIT).

```

This `README.md` file provides an overview of the project, instructions on how to use the functions, and an example of what the output looks like.
