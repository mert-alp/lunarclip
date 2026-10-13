# LunarClip — Ban-Proof Reddit & Community Launch Kit

This kit provides battle-tested posting strategies, target subreddits, post copy, and comment response scripts to drive organic traffic and backlinks to **LunarClip** ([lunarclip.com](https://lunarclip.com)) without getting flagged or banned by Reddit's AutoModerator.

---

## 🛡️ The 5 Golden Rules to Avoid Bans on Reddit

1. **The 9:1 Community Ratio**:
   Reddit enforces a strict ratio: at least 9 helpful, authentic community comments for every 1 self-promotional link or mention. Never create a new account just to post links.
2. **Account Warmup**:
   - Minimum account age: 30 days.
   - Minimum comment karma: 50+ karma (gained from participating in gaming, tech, or creator subreddits).
3. **Use the "Safe Gateway" (GitHub Bridge)**:
   - When posting in subreddits with strict commercial link filters, link to your public repository: `https://github.com/mert-alp/lunarclip` instead of a direct commercial domain. AutoModerator rarely blocks GitHub repositories, and your GitHub README immediately funnels traffic to `lunarclip.com`.
4. **Disclose Transparently**:
   - In comments, always state: *"Disclaimer: I built LunarClip (https://lunarclip.com)..."*. Communities respect creators; they ban stealth marketers.
5. **Rate Limiting**:
   - Never post the same text to more than 1 subreddit on the same day. Space out submissions by 48–72 hours across different subreddits.

---

## 🎯 Target Subreddits

| Subreddit | Subscribers | Allowed Content | Best Angle / Flair |
| :--- | :--- | :--- | :--- |
| **r/SideProject** | 200k+ | Direct project showcases | "I built this" / Project / Feedback |
| **r/SaaS** | 180k+ | Founder stories & pricing breakdowns | Showcase / Growth / Feedback |
| **r/indiehackers** | 80k+ | Technical and business learnings | Product / Launch |
| **r/windowsapps** | 50k+ | Windows desktop utilities | New App / Release |
| **r/software** | 150k+ | Software recommendations | Recommendation / Utility |
| **r/NewTubers** | 350k+ | Value-first guides (**NO links in post**) | Guide / Discussion |
| **r/streaming** | 120k+ | Streamer workflows (**NO links in post**) | VOD editing / Advice |
| **r/podcasting** | 100k+ | Podcast clip production (**NO links in post**) | Production / Tips |

---

## 📝 Ready-to-Copy Post Copy

### Post 1: r/SideProject & r/SaaS (Founder Showcase)

**Title**: Tired of 1-hour cloud uploads and credit burn on OpusClip, I built a local-first Windows clipper (LunarClip)

**Body**:
```markdown
Hey everyone,

If you produce or edit long-form content (2+ hour podcasts, Twitch VODs, esports games), you've probably tested cloud AI clippers like OpusClip or Vizard. 

While they're fine for 5-minute clips, I kept hitting two major walls with long footage:
1. **The Upload Bottleneck**: Waiting 45 minutes to upload a 20GB recording to a browser just to see if the tool could find anything.
2. **The "Per-Minute Credit Burn"**: A 2-hour video burns 120 credits. If you don't use them, credits expire, and projects disappear when subscriptions pause.

To solve this, I spent the last few months building **LunarClip** (https://lunarclip.com) — a native Windows desktop app built around a **local-first engine**:

- 🔒 **Video stays on your machine**: Media extraction (FFmpeg) and transcription (faster-whisper in 46+ languages) run locally on your PC. Only the lightweight text transcript is sent for AI semantic scoring.
- 🎯 **Measured Highlights**: Rather than relying purely on an AI "predicting virality", it reads YouTube audience replay curves (what viewers actually rewound to), acoustic spikes, and scene cuts.
- 📐 **Adaptive Framing Presets**:
  - *Podcasts*: Splits the screen automatically when two people speak and cuts to whoever is talking.
  - *Gaming*: Detects facecam and places it on top (~30%) with gameplay below (~70%).
  - *Sports*: Wide tracking that follows the ball and nearby action instead of jarring tight zooms.
- 💳 **Flat Monthly Quotas**: No expiring per-minute tokens. Free tier includes 5 videos/month.

We've also put together an open showcase and community issue tracker on GitHub: https://github.com/mert-alp/lunarclip

I’d love to get feedback from fellow creators and devs: how do you currently handle vertical reframing, and what layout styles do you think are most effective?
```

---

### Post 2: r/NewTubers & r/streaming (Value-First Guide — Ban-Proof)
*(Notice: NO direct link in the post body. This completely bypasses auto-moderation. When users reply asking for the app, you provide the link in the comments.)*

**Title**: Why cloud clippers struggle on long livestreams (and how local processing cuts the workflow time by 80%)

**Body**:
```markdown
Hey creators,

If you stream on Twitch or YouTube and try turning 3-hour VODs into vertical Shorts and TikToks, you've probably noticed that most cloud clippers feel sluggish and expensive. 

I spent the past few months profiling why this happens and how you can optimize your clipping workflow:

### 1. The Real Bottleneck is Bandwidth, Not AI
Cloud clippers require you to upload your full uncompressed video file to a remote server. For a 3-hour 1080p stream (often 10–25 GB), an average home internet connection spends 30–60 minutes just on the upload bar before transcription even starts.
*Solution*: Running speech-to-text locally (tools like faster-whisper on an Nvidia or modern CPU) takes 2–4 minutes for an entire hour of audio, with zero upload wait time.

### 2. Why "Predicted Virality Scores" Often Miss
Many clippers score clips on a generic 0–100 scale using an LLM's guess of what's "trendy". In practice, a noisy throw-in in soccer or quiet farming in League of Legends can get scored high by mistake.
*What works better*: Look at **Audience Replay Heatmaps** (the most-replayed graph on YouTube). If human viewers rewound to a specific 30-second window, that's a verified high-interest moment.

### 3. Layout Matching
One-size-fits-all center crops ruin gameplay:
- Fast FPS games (Valorant/CS) need the webcam pinned top (~30%) and gameplay centered (~70%).
- Sports need a loose wide track that follows the ball rather than punching in.

I ended up coding a standalone Windows tool called LunarClip around these principles to process long files locally without burning subscription credits. 

For those of you regularly cutting shorts: do you prefer manual timeline editing in Premiere/DaVinci, or automated clippers with manual tweaking? Happy to answer questions about local transcription pipelines!
```

---

### Post 3: Comment Interception (For People Asking "Best OpusClip Alternative?")

**Comment Body**:
```markdown
If you're on Windows and tired of per-minute credit limits or waiting for multi-gigabyte uploads to finish, check out **LunarClip** (https://lunarclip.com).

*Full disclosure: I'm the developer.*

We built it specifically for people with long recordings:
- Your source video never leaves your PC (transcription runs locally with faster-whisper in 46+ languages).
- Built-in framing presets for podcast split-screen and gaming (webcam overlay).
- Flat monthly allowances rather than expiring credits. 

Free tier gives you 5 videos a month to test the reframing on your own hardware.
```

---

## ⚡ Hacker News: Show HN Template

- **Submission URL**: [https://news.ycombinator.com/submit](https://news.ycombinator.com/submit)
- **Title**: `Show HN: LunarClip – Local-first AI video clipper for Windows`
- **URL**: `https://lunarclip.com` (or link to `https://github.com/mert-alp/lunarclip`)

**First Comment (Self-text)**:
```text
Hi HN,

I built LunarClip (https://lunarclip.com), a Windows desktop app that transforms long video files and YouTube links into vertical 9:16 clips for Shorts, TikTok, and Reels.

Most existing video clippers operate as cloud services. While cloud works well for short web clips, it breaks down for 2–8 hour livestreams, esports matches, and long podcasts. Uploading a 20GB recording over typical home broadband takes an hour before processing begins, and cloud GPU rendering costs force vendors into restrictive per-minute credit models.

LunarClip uses a local-first pipeline:
1. Media demuxing and inspection run locally via FFmpeg / ffprobe.
2. Speech transcription runs on-device using faster-whisper (CTranslate2), supporting 46+ languages.
3. Only the lightweight text transcript is sent to our backend for semantic moment scoring, hook generation, and layout orchestration.
4. Video rendering and word-level karaoke caption burning execute locally.

Because heavy video frames never leave the user's machine, we avoid large cloud egress/storage costs and can offer straightforward monthly allowances without credit expiration.

Public repo and technical documentation: https://github.com/mert-alp/lunarclip

I'd appreciate any feedback on our local pipeline architecture or desktop workflow!
```
