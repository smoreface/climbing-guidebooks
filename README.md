# Climbing Guidebooks Dataset

This repo provides a CSV dataset about guidebooks published about climbing areas in the United States of America (USA). 

## How was the data collected?

An initial collection of all guidebooks from three major retailers:

- Rock and Snow
- REI
- Amazon

The Amazon guidebooks were gathered from a search for "guide" in the category **Books : Sports & Outdoors : Mountaineering : Rock Climbing**

Only climbing guides have been collected. This includes rock climbing, bouldering, ice climbing, and the occasional mountaineering guide if it mentions climbing. 
Hiking guides and mountaineering guides that do not mention climbing have been excluded.

The initial dataset was then enhanced with data from other retailers and publishers of climbing guidebooks:

- [Eastside Sports](https://eastsidesports.com/collections/climbing-guidebooks)
- [Fixed Pin Publishing](https://www.fixedpin.com/collections/climbing)
- [Ground Up Publishing](https://grounduppublishing.com/)
- [Climbing Wyoming](https://www.climbingwyoming.com/guidebooks/)
- [SuperTopo](http://www.supertopo.com/topostore.html)
- [Big Willi Mountaineering Co](https://bigwillimc.com/)
- [Neptune Mountaineering](https://neptunemountaineering.com/collections/climbing-guide)
- [Mad Rock Climbing](https://madrock.com/collections/guidebooks)
- [Falcon Guides](http://falcon.com/books/)
- [Sharp End Publishing](https://stores.sharpendbooks.com/)
- [Wolverine Publishing](https://www.wolverinepublishing.com/product-category/guidebooks/rock-climbing/)
- [K. Daniels Publishing](https://kdanielspublishing.com/cart/index.php/guide-books.html)

Some rabbit holes were followed when searching for data about the books on the initial list, leading to various other sources such as self published books and posts on Mountain Project about guidebooks:

- [Mountain Project list of out of print Colorado guidebooks](https://www.mountainproject.com/forum/topic/105084501/out-of-print-colorado-guidebooks)
- [Mountain Project post on Southern Nevada Guidebooks](https://www.mountainproject.com/books/113755154)

## About the dataset

This dataset is provided as a comma-separated values (CSV) file with the following columns:

| column name | format | details|
| -- | -- | -- | 
| title | string | title of the guidebook |
| year | string | year the guidebook was published |
| authors | multi-value comma-separated strings | author(s) of the guidebook |
| note | string | miscellaneous information about the guidebook, such as whether it's out of print or digital only ||
| edition | integer | number of the book edition. For example, 1 for the first edition of a book. |
| editors | multi-value comma-separated strings | editor(s) of the guidebook, if known |
| publisher | string | publisher of the guidebook |
| ISBN | string | ISBN-13 of the guidebook, occasionally ISBN-10. |

### Notes about missing data 

Given this initially standard and then chaotically deviating methodology, 
there are certainly gaps in this dataset in terms of:

- Edition coverage. Not all book editions are captured.
- ISBNs. Not all ISBNs could be identified, and not all books have ISBNs, especially self-published books. Even when the ISBN exists, it might not be clearly documented online.
- Years. Not all publication years could be identified.
- Publishers. Not all book publishers could be identified.
- Editors. Data on editors was collected only when easily available and known.

Because this research was conducted using what is available from online retailers, missing information that might be available to book owners was often unable to be verified (the data collectors do own some guidebooks!) . 

If you want to help, see [How to contribute to this dataset](#how-to-contribute-to-this-dataset).

### Notes on standardization of the data 

In some cases, the data in the dataset might not match the ISBN record data or information for a specific book or edition. 
Some decisions were made to standardize the data to make comparisons easier to perform. For example:

- Author name spelling. For authors with multiple books and multiple name spellings, the most common name spelling was chosen to represent the author in the dataset. For example, Peter Hubbell (sometimes Hubbel).
- Self published books were noted as "Self Published", rather than listing the author name.

## Who collected the data?

- Kimbrough Moore, climbing guidebook author and philosophy professor, collected the initial dataset.
- Sarah Moir, technical writer and data analysis dabbler, expanded and standardized the dataset.

## Why was the data collected? 

To gather a better understanding of who is writing climbing guidebooks.

## How to contribute to this dataset

There are a lot of gaps in this dataset, and we welcome contributions of:

- Guidebooks missing from this dataset. Please include as many column values as possible.
- Data missing for guidebooks in this dataset, such as year, publisher, or editor.

How you contribute depends on how comfortable you are using GitHub:

- If you're comfortable with GitHub, open a pull request to add or update the data in the CSV file.
- If you have a GitHub account but don't want to open a pull request, open a GitHub issue with as much detail as possible about the data that you want added.

To ensure data integrity, include verifying information such as an ISBN number, or a photo of a publishing page for the guidebook.

## How to cite this dataset

Authors: Kimbrough Moore and Sarah Moir
Title: USA Climbing Guidebook Dataset
Year Created: 2023

This dataset uses the MIT license. 
