
# Annotations file (anim400K_anntions.json, 266Mb)

The annotations are stored in an omnibus annotations file, with the following form:
```json
{
  'show_key': {
    'show': str (The name of the show),
    'season': str (The name of the season),
    'link': str (A URL to the season information),
    'type': str (The type of anime),
    'status': str (If the anime has finished),
    'genres': [str] (The genres present in the anime),
    'themes': [str] (The themes present in the anime),
    'score': float (The average anime score),
    'scored_by': int (The number of scorers),
    'rank': int (The rank, by score, at the time of data collection),
    'popularity': int (The rank, by followers, at the time of data collection),
    'members': int (The number of followers),
    'favorites': int (The number of people who favorited the show),
    'episode_num': int (The number of episodes),
    'aired': str (The air date),
    'premiered': str (The premeire date),
    'broadcast': str (When the show aired),
    'producers': [str] (The producers for the show),
    'licensors': [str] (The licensors for the show),
    'studios': [str] (The studios for the show),
    'source': str (The source material for the show),
    'avg_duration': str (The length of each episode),
    'rating': str (The content rating for the show),
    'related_anime': {} (Related shows),
    'opening_themes': [str] (The list of opening themes for the show),
    'ending_themes': [str] (The list of ending themes for the show),
    'staff': [str] (A list of staff members for the show),
    'background': str (Background information for the show),
    'synopsis': str (Show synopsis),
    'characters': {
      'Character Name': {
        'description': str (A description of the character),
        'role': str (The role, main/supporting),
        'pic_urls': [str] (A list of IDs corresponding to character pictures),
        'Voice Actors': [str] (A list of voice actors for the character,
      }
    },
    'episodes': {
      'episode_number': {
        'url': str (A link to the episode information),
        'ratings': {
          'score': {'ratio': float (percent of voters for this score), 'number_of_voters': float (Number of people voting for this score)},
          ...
         },
        'jp_video_id': str (The ID of the full JP video),
        'en_video_id': str (The ID of the full EN video),
        'synopsis': str (The episode synopsis)
        'clips': [
          {
            "jp_clip": str (The ID of the JP clip),
            "en_clip": str (The ID of the EN clip),
            "jp_text": str (The ASR for the JP audio),
            "en_text": str (The ASR for the EN audio),
            "jp_start_time": str (A timestamp in the JP video for the start of the clip),
            "jp_end_time": str (A timestamp in the JP video for the end of the clip),
            "en_start_time": str (A timestamp in the EN video for the start of the clip),
            "en_end_time": str (A timestamp in the EN video for the end of the clip),
            "speakers": [str] (The automatically recognized speaker IDs present in the clip at an episode level),
          },
          ...
         ],
      }
      ...
  }

}
```

# Audio Clips (34Gb)

The audio clips are stored in a .tar.gz file, containing the following form:
```
anim400k_audio_clips/
    {id_folder}/{id}
```
For example, the audio clip ID `db/db019ebb-088c-4850-b791-de097303264d` is stored in `anim400k_audio_clips/db/db019ebb-088c-4850-b791-de097303264d.mp3`.

# Video Clips (199Gb)

The video clips are stored in a .tar.gz file, containing the following form:
```
anim400k_video_clips/
    {id_folder}/{id}
```
For example, the video clip ID `db/db019ebb-088c-4850-b791-de097303264d` is stored in `anim400k_audio_clips/db/db019ebb-088c-4850-b791-de097303264d.mp4`.

# Character Pictures (262Mb)

```
anim400k_character_pics/
    {id_folder}/{id}
```
For example, the character picture ID `e/e2def42e-63fe-4e06-b474-314e1d29382c` is stored in `anim400k_character_pics/e/e2def42e-63fe-4e06-b474-314e1d29382c.jpg`.
