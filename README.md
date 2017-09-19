# CMCCKL Sunday Service Automation
Automate weekly Sunday worship service 

## Features
- [ ] Consolidate current slides stored in Dropbox into a database
- [ ] Generate slides from the database
- [ ] Crawl hymnal.org to save into the database
- [ ] Generate slides and save as PowerPoint
- [ ] Multilingual slides support (English, Chinese, Malay and more)

## Proposed tech stack
- Heroku + mLab
- NodeJS backend with Koa + MongoDB
- Create React App front end
  - Search slides
  - Select slides to combine or generate slides as PowerPoint

## Todo
- [ ] Script/Engine to convert existing slides into database entry
- [ ] Database document schema (slides/song object schema) 
Example: 
```
{
  "title": "Amazing Grace",
  "lyrics": {
    "en": {
      "v1": [
        "Amazing grace! how sweet the sound, That saved a wretch; like me!",
        "I once was lost, but now am found, Was blind, but now I see."
      ],
      "v2": [
        "’Twas grace that taught my heart to fear, And grace my fears relieved;",
        "How precious did that grace appear The hour I first believed!"
      ],
      ...
    },
    "cn": {
      "v1": [
        "奇异恩典 何等甘甜 我罪以得赦免",
        "前我失丧 今被寻回 瞎眼今得看见"
      ],
      "v2": [
        "如此恩典 使我敬畏使我心得安慰",
        "初信之时 即蒙恩惠 真是何等宝贵"
      ],
      ...
    }
  }
}
```

## Existing solution
1. [OpenLP](https://openlp.org/)
> [Developer portal](https://openlp.io/)
