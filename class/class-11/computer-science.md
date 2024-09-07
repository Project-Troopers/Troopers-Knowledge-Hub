# Computer Science

Welcome to the Computer Science section! In this course, we will explore the fascinating world of computers, their components, and the principles that govern their functioning. Computer Science is the scientific study of computers and their applications, which play a crucial role in our daily lives. Whether it is the software that powers our smartphones or the algorithms that drive the internet, understanding the underlying concepts of computer science is essential.

[CBSE Computers 2023-2024 Curriculum.pdf](https://res.craft.do/user/full/34ae8ebc-d508-7305-20e2-17e06364862c/doc/3491F8B8-527B-4029-A8C5-FBF1AF7CCE2D/bcebbf97-168c-fc90-e430-5eb46e6375df/r4Tax4XSBfrmyUy04QilNpjucTCLcTJZcVZ5YYPKIx0z/Files%20from%20iOS.pdf)

## Some good materials

{% embed url="https://www.comparitech.com/blog/information-security/encryption-hashing-salting/" %}

## Revision

[Computer Science - New Learning Standards Framework Questions - CBSE.pdf](https://res.craft.do/user/full/34ae8ebc-d508-7305-20e2-17e06364862c/doc/3491F8B8-527B-4029-A8C5-FBF1AF7CCE2D/6EF7ADBD-739B-44C0-907F-1CF79D29DDE7\_2/mNqr7WvAwlLEzdAvzQnWgpAoyqQC9BxZTxmv2LJKHxwz/Computer%20Science%20-%20New%20Learning%20Standards%20Framework%20Questions%20-%20CBSE.pdf)

## Miscellaneous Examples

1. Script to download a PDF hosted on Google Drive with the download button disabled, as images and download it as a zip onto your computer.

```javascript
if (window.trustedTypes && window.trustedTypes.createPolicy) {
  window.trustedTypes.createPolicy('default', {
    createHTML: (string) => DOMPurify.sanitize(string, { RETURN_TRUSTED_TYPE: true }),
    createScriptURL: string => string,
    createScript: string => string,
  });
}

let jsZip = document.createElement("script");
jsZip.onload = function () {
  let zip = new JSZip();
  let elements = document.getElementsByTagName("img");

  for (let i in elements) {
    let img = elements[i];

      if (!/^blob:/.test(img.src)) {
        console.log("invalid src");
        continue;
        }

      let can = document.createElement('canvas');
      let con = can.getContext("2d");
      can.width = 1600;
      can.height = 900;
      con.drawImage(img, 0, 0, 1600, 900);

      let imgData = can.toDataURL("image/jpeg", 1.0);

      // Get a unique name for each image
      let imgName = `image_${i}.jpg`;

      // Add the resized image to the zip file
      zip.file(imgName, imgData.split('base64,')[1], { base64: true });
      }

  // Generate the zip file and trigger the download
  zip.generateAsync({ type: "blob" })
  .then(function (content) {
  // Trigger download
    let link = document.createElement("a");
    link.href = URL.createObjectURL(content);
    link.download = "images_Stella.zip";
    link.click();
    });
};

jsZip.src = 'https://cdnjs.cloudflare.com/ajax/libs/jszip/3.1.5/jszip.min.js';
document.body.appendChild(jsZip);
```

## Record work

The following are the programs to be written in the record and submitted:

*   Record Entry no. 4

    Page 279, question 3.
*   Record Entry no. 5

    Page 305, program 9.11
*   Record Entry no. 6

    Page 313, question 11
*   Record Entry no. 7

    Page 352, program 10.10
*   Record Entry no. 8

    Page 352, program 10.11
*   Record Entry no. 9

    Page 385, program 11.12
*   Record Entry no. 10

    Page 395, question 18
*   Record Entry no. 11

    Page 439, question 21
*   Record Entry no. 12

    Page 441, question 25.

Cover your record with brown paper.

## Aim

Throughout this course, we will delve into various topics such as programming languages, data structures, algorithms, and computer networks. We will learn the fundamentals of problem-solving through programming and explore how computers can effectively process and manipulate data. Additionally, we will analyze computer systems and architecture to understand how they function at a hardware level.

By the end of this course, you will not only have a strong foundation in computer science principles but also be equipped with practical skills that will enable you to develop your own software applications. So, get ready to embark on this exciting journey into the world of computers and unlock the infinite possibilities that computer science has to offer.
