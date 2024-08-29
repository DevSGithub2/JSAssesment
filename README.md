# JavaScript Assessment

A JavaScript project for creating, listing, and managing NFTs with metadata.


## Description

This project is a JavaScript assessment focusing on creating and managing NFTs. The provided code allows you to mint NFTs, list all NFTs with their metadata, and get the total number of NFTs minted. Each NFT has metadata including name, age, eyecolor, and accessories.

## Features

- **Mint NFTs**: Create and add new NFTs with specified metadata.
- **List NFTs**: Print metadata of all NFTs to the console.
- **Get Total Supply**: Return the total number of NFTs minted.

## Instruction

### * Assessment Requirements

1. Create a variable that can hold a number of NFT's. What type of variable might this be?
2. Create an object inside your mintNFT function that will hold the metadata for your NFTs. 
   The metadata values will be passed to the function as parameters. When the NFT is ready, 
      you will store it in the variable you created in step 1
3. Your listNFTs() function will print all of your NFTs metadata to the console (i.e. console.log("Name: " + someNFT.name))
4. For good measure, getTotalSupply() should return the number of NFT's you have created


### Code 
```

// Create a variable to hold your NFTs
const NFTs = [];

// Function to mint a new NFT
function mintNFT(_name, _age, _eyecolor, _accessories) {
    const NFT = {
        name: _name,
        age: _age,
        eyecolor: _eyecolor,
        accessories: _accessories
    };
    NFTs.push(NFT);
    console.log("Minted: " + _name);
}

// Function to list all NFTs
function listNFTs() {
    for (let i = 0; i < NFTs.length; i++) {
        console.log("\nID: " + (i + 1));
        console.log("Name:\t\t " + NFTs[i].name);
        console.log("Age:\t\t " + NFTs[i].age);
        console.log("Eyecolor:\t " + NFTs[i].eyecolor);
        console.log("Accessories:\t " + NFTs[i].accessories);
    }
}

// Function to get the total number of NFTs minted
function getTotalSupply() {
    console.log("\nTotal NFTs Minted: " + NFTs.length);
}

// Call functions to demonstrate functionality
mintNFT("Ravi", "20Y", "brown", "bracelet");
mintNFT("Adarsh", "20Y", "brown", "bracelet");
mintNFT("Akshay", "20Y", "brown", "bracelet");
mintNFT("Dev", "20Y", "brown", "bracelet");
listNFTs();
getTotalSupply();


```

## Authors

- Dev Sagar - [@DevSGithub2](https://github.com/DevSGitub2)

### Thank you for checking out this project. Your feedback and contributions are appreciated!
