### Workshop 13: Uploading images on blockchain
This Exercise will be precisely to create uploading engine with transactions. image will be split down of severul chunks
of data and each chunk will be uploaded on the separate account. Then the client library will be combining all the different data accounts
and combining data stored there - displaying the stored image.

I Think this will be a good challenge for seminars because it consists of several parts:
* implementing and deploying the program
* spliting and uploading images
* managing several different accounts
* fetching images by their on chain metadata, for example **owner address**
* calculating the costs and `upload/download` time to finally come to conclusion why is this approach a bad idea.

**The Program**\
The program functionality will be simple it only will have a few instructions to manage data accounts. also each image will
have a separate metadata account for additional information, like uploader address.

**The Client Code**\
The main challenge in this assignment will be in client code. uploading image data in several different transactions might be 
a bit tricky because we need to account for transaction skipping. there are several approaches, most naive one being
waiting for confirmation of one transaction before proceeding with another. (we will discuss better approaches within the workshop)

Also images will be stored in different data accounts and metadata accounts will be responsible on storing the information
about where is data located.

The main idea of this workshop is not teaching real world examples but showing what capabilities does Solana have in terms of
data management.

