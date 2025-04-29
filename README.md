# Final-Project
For my project, I picked a spotify artist dataset. It had a lot of categories, but I narrowed it to artist names and their streams. 
Original dataset: 
[Spotify Artist Stats](https://www.kaggle.com/datasets/adnananam/spotify-artist-stats)

#Code Structure

Parsing: The data was a csv file, uploaded using DictReader. Each row is stored as a dictionary with the keys "artists" and "streams"
Each row is stored as a list, labeled "data."

Sorting: I used both bubble sort and selection sort. Each took the data and a key (I chose to use streams).
Each sorting method outputed the data, sorted from least amount of streams to most. 

Searching: I wanted to use binary search, but since that requires a sorted list, I would have had to sort the data
alphabetically based on artist. Which seemed too complicated. So I opted for linear search. The function takes an artist's name, 
and outputs it along with the artist's streams. 

Top 5 Feature: I chose to use a heap, and built it from the bottom 5 artists of my bubble sorted data (these would be the artists with most streams).
They are put in a max heap. There are functions called heapify and build_max_heap to help mantain max heap structure. 

It's all in one file (a script with sections), in order to stay organized. 

#Time Complexity Analysis
