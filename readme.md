
# ❄️ MERRY CHRISTMAS ❄️

Sometimes you just want to send your clients a really nice, simple end of year video. It has to be a little more festive than a simple youtube embed. It's just something pretty and simple. No frills, no thrills, just 5 minutes in HTML and a few seconds to push out to an S3 Bucket or drop on a flash drive.

<img alt="Image" src="https://github.com/user-attachments/assets/e79c83c4-530f-4f8d-9da7-6871483b219e" />

This is just that. Built with TailwindCLI and nothing else.

## 🎞️ Background & Video Customization

Changing out the background and video couldn't be easier! Especially as this repo doesn't ship with a working video.

To change out the background, either:

1. Replace /assets/bg.jpg with a different image.
2. Edit line 11 in Video_Player.html:
```html
    <div class="bg-[url(bg.jpg)] bg-cover w-full min-h-screen m-0 p-0">
```

Replace bg.jpg with a path to your image.

To change out the videos:

1. Put your videos in: /assets/videos/.
2. Edit lines 14 & 15 in Video_Player.html
```html
    <source src="assets/videos/VIDEO_4K_HERE.webm" media="(width >= 2000px)" />
    <source src="assets/videos/VIDEO_1080P_HERE.webm" />
```

Replace the appropriate file names for your video files. The top file will play on screens over 2,000 pixels wide and the bottom file will  play for screens less than 2,000 pixels wide.


## ✏️ CSS Customization

Download the repository and then run:

```shell
npm install
```

This will grab the  TailWindCLI so you can use all their classes and have slim/efficient CSS. Keep your terminal open, you'll need to run:

```shell
npx @tailwindcss/cli -i ./assets/base.css -o ./assets/styles.css
```

This will generate new CSS based on your HTML. **If you don't run it for every change, that CSS will never get loaded.**


## License

