
library(tidyverse)
library(spotifyr)

# Set Spotify access variables (every time)

Sys.setenv(SPOTIFY_CLIENT_ID = '8757ad55abf941a8897908a6d2e1e1da')
Sys.setenv(SPOTIFY_CLIENT_SECRET = 'e92c425ebe9049e49373a8153a6c891f')

# Work with spotifyr. Note that playlists also require a username.

juditha <-
  get_track_audio_features(
    c('2M5b9YLAgFroqWzeaZf86e', '3DBKc4ioGnMQLlbGQcFDIO')
  )
alla <- get_album_tracks('7oI0E3DdTbD85rhMg19GSU')
gilberto <- get_artist_audio_features('gilberto gil')
disney <- get_playlist_audio_features('128899670', '5NtjgKz4doejP5HJtKXFcS')

# Summarise key patterns

gilberto %>% summarise(M = mean(danceability), SD = sd(danceability))
disney %>% summarise(M = mean(danceability), SD = sd(danceability))

# Questions to answer during the lab
#
# 1. Is 'Let It Go' typical or atypical of Disney hits, with respect to the
#    features in the Spotify API?
# 2. What are the similarities and differences between the 'This is Cazwell'
#    and 'This is Eminem' playlists on Spotify? (Be warned that the lyrics are
#    explicit, like much hip hop, but you don't need to listen.)

Cazwell <- get_playlist_audio_features('spotify','37i9dQZF1DZ06evO3u4FEc')

# Computational Opdracht

PersianRock<- get_playlist_audio_features('ehsancinematic', '1Osyac6DOmnjH8XxSSR9XP')
Rock<- get_playlist_audio_features('spotify', '37i9dQZF1DX49jUV2NfGku')

Hello there, welcome to my page! I’ve chosen to compare the score of horror and romance . For horror i’ve chosen for the classic movie ‘’The Shining’’ from 1980, directed by Stanley Kubrick, and for romance ive chosen "Amélie’’ from 2001, directed by Jean-Pierre Jeunet. These movies are highly rated on IMDB (whitin own genre) and therefore representable for it’s genre. I have chosen for horror because i think it will be interesting to see the results, especially if you compare it to its opposite genre: romance.
For this case i want to use Rmarkdown in combination with the Spotify API. For the storyboard i'm gonnna use flexdashboard. 
Tracks that are interested for this research are both intro themes for each movie. 
A line I wrote on my local computerkjkj
A line I wrote on my local computer
A line I wrote on my local computer
bkasjkjkj
hoihoihoi
adding a line
this is a line from Rstudio