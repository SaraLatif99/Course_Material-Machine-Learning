Given only inputs (no categories), automatically discover representations, correlations, features, structure, etc.

The aim is to find the regularities in the input; density estimation. There is a structure to the input space such that certain patterns occur more often than others, and we want to see what generally happens and what does not. 

Group and interpret data based only on input data; data driven.

1. Clustering

Given customer data containing demographic data and past transactions, determine distribution of the profile of its customers, to see what type of customers frequently occur. You could use customer segmentation to group customers with similar data. You could use customer relationship management which services and products to advertise to each customer segment. You may be able to determine a niche in the market by observing the outliers, which can be further targeted in a unique way. 

Another example is image compression. The input instances are image pixels represented as RGB values. The ML model could group pixels with similar colors in the same group, and such groups correspond to the colors occurring frequently in the image. If in an image, there are only shades of a small number of colors, and if we code those belonging to the same group with one color, for example, their average, then the image is quantized. For example, if we have an image with 24 bits to represent the respective 16 million colors. If there are various shades of blue in different parts of the image, we can use the same average blue for each pixel, then we only need 6 bits instead of 24 bits. We lose the details in the image but gain space in storage and transmission. The goal is to identify higher-level regularities like texture or object by analyzing repeated image patterns, which could compress better than at the pixel level while still maintaining the description of the scene. Another example would be haveing an image of a document, which contains a 16 x 16 bitmap of letters, which take 32 bytes, while the ASCII code of the letters only takes 1 byte. We could compress each bitmap letter into a byte.

Another example is document clustering. News reports can be subdivided as those related to politics, sports, fashion, arts, etc. We could represent a document as a bag of words, which is a predefine a lexicon of N words. Each document is an N-dimensional binary vector whose element i is 1 if word i appears in the document. Suffixes are removed to prevent duplicates and prepositions are removed because they are not informative. Documents are then grouped depending on the number of shared words. Lexicon choice will affect the output greatly.

Another example is alignment, which is matching one DNA sequence to another. There are many template strings to match against, and there may be deletions, insertions, and substitutions. Clustering is used in learning motifs, which are sequences of amino acids that occur repeatedly in proteins. 
