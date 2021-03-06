# The Music App

https://meeday.github.io/The-Music-App/

## Summary

A webapp that searches for music by track, album, or artist. Enter in your search query and access a wealth of information from reputable sources.

## Contents

- [Planning](#planning)
  - [User Story](#user-story)
  - [Acceptance Criteria](#acceptance-criteria)
  - [Wireframes](#wireframes)
  - [APIs](#apis)
- [Features](#features)
  - [Results Pages](#results-pages)
    - [Track Search](#track-search)
    - [Album Search](#album-search)
    - [Artist Search](#arist-search)
  - [Modals](#modals)
    - [Track Modal](#track-modal)
    - [Album & Artist Modals](#album-artists-modal)

## Planning

### User Story

AS an avid music fan,
I WANT an App that gives me information on songs
SO THAT I can learn more about the artists and their work

### Acceptance Criteria

GIVEN that I input a valid name  
WHEN I enter a track name  
THEN I am presented with detailed information about the track  
WHEN I enter an album name  
THEN I am presented with info on the album and a list of songs in it  
WHEN I enter an artist name  
THEN I am presented with a bio, some info about them, and discography

### Wireframes

![image](https://user-images.githubusercontent.com/59972622/80771729-3c14e880-8b4c-11ea-936d-c620bbad988c.png)
![image](https://user-images.githubusercontent.com/59972622/80771761-5a7ae400-8b4c-11ea-8554-7d0bb3b74e73.png)
![image](https://user-images.githubusercontent.com/59972622/80771774-5f3f9800-8b4c-11ea-9281-97c70ca5f2e5.png)
![image](https://user-images.githubusercontent.com/59972622/80771775-61095b80-8b4c-11ea-970f-dbd6875e8b3c.png)

### APIs

#### Third Party

##### LastFM

The main API, used to retrieve artist info and to fill out the search result pages

##### audd.io API

Used to retrieve song lyrics on request.

Used to retreive upcoming shows and concerts related to the artist

### CSS Framework

Materialize css is used for most of the styling with some custom css to support it

## Features

### Results Pages

With all search result pages the user will be able to click on arist/album/track names in the results to open a [modal](#modals) with more info on that item.

#### Track Search

This will display the top 10 search results. The user can then click to select which track they want. This will then show them the track info.

#### Album Search

This will return the album with:

- Artist
- Brief summary (if available)
- Tracklist

#### Artist Search

When selecting artist and searching the user will be presented with artist info:

- Bio
- Top Albums
- Top Tracks

### Modals

These are shown whenever a user clicks on a link in the [results pages](#results-pages) and have been implimented so that a user won't lose their original search if they go down the 'rabbit hole' and click numerous links. Any link clicked within a modal will refresh/change the modal to display the new info.

#### Track Modal

- Track
- Album title with cover
- Artist name
- Lyrics

#### Album & Artist Modals

These are designed the same as the existing results pages.
