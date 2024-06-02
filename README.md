# Javascript-Assessment
# NFT Minting Application

## Overview

This JavaScript application allows users to mint, list, and track the total number of NFTs created. An NFT (Non-Fungible Token) in this context is represented by a simple object containing metadata such as title, description, and an image URL.

## Features

1. **Mint NFTs**: Create new NFTs with specific metadata and store them in a collection.
2. **List NFTs**: Display the metadata of all minted NFTs.
3. **Total Supply**: Get the total number of NFTs created.

## Code Explanation

### NFT Class

The `NFT` class is a blueprint for creating NFT objects. Each NFT object contains the following properties:
- `title`: The title of the NFT.
- `description`: A description of the NFT.
- `imageUrl`: A URL pointing to an image representing the NFT.

```javascript
class NFT {
  constructor(title, description, imageUrl) {
    this.title = title;
    this.description = description;
    this.imageUrl = imageUrl;
  }
}
```

### NFT Collection

A variable `myNFTs` is used to store all minted NFTs. It is an array that holds `NFT` objects.

```javascript
const myNFTs = [];
```

### Minting Function

The `mintNFT` function creates a new `NFT` object with the provided metadata and adds it to the `myNFTs` array.

```javascript
function mintNFT(title, description, imageUrl) {
  const nft = new NFT(title, description, imageUrl);
  myNFTs.push(nft);
}
```

### Listing Function

The `listNFTs` function iterates over the `myNFTs` array and prints the metadata of each NFT to the console.

```javascript
function listNFTs() {
  for (let i = 0; i < myNFTs.length; i++) {
    const nft = myNFTs[i];
    console.log("Title: " + nft.title);
    console.log("Description: " + nft.description);
    console.log("Image URL: " + nft.imageUrl);
    console.log("----------------------");
  }
}
```

### Total Supply Function

The `getTotalSupply` function returns the total number of NFTs created by returning the length of the `myNFTs` array.

```javascript
function getTotalSupply() {
  return myNFTs.length;
}
```

### Example Usage

The following code demonstrates how to mint NFTs, list them, and get the total supply of NFTs:

```javascript
// Minting NFTs
mintNFT("Artwork", "Abstract painting", "https://example.com/image1.png");
mintNFT("Photography", "Landscape photo", "https://example.com/image2.png");
mintNFT("Digital Art", "3D rendered artwork", "https://example.com/image3.png");
mintNFT("Blender Art", "Blender artwork", "https://example.com/image4.png");

// Listing all NFTs
console.log("Listing NFTs:");
listNFTs();

// Displaying the total number of NFTs created
console.log("Total NFTs created: " + getTotalSupply());
```

## How to Run

1. Copy the entire code into a JavaScript file (e.g., `nft.js`).
2. Run the JavaScript file using a Node.js environment or in the browser console.

## Conclusion

This application provides a simple yet functional implementation for creating, listing, and tracking the total number of NFTs. It serves as a basic example and can be expanded with additional features like editing NFT metadata, deleting NFTs, or integrating with a blockchain for actual NFT minting and trading.
