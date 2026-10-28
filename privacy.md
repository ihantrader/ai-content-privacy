# Privacy Policy — AI Content

_Last updated: October 28, 2026_

AI Content (the "Application") is a personal desktop tool its owner uses to research topics, make videos and publish them to the owner's own YouTube channel. It runs only on the owner's computer. It is not offered to other people, has no user accounts and no servers of its own, and the owner is its only user.

This policy explains what data the Application gets from Google and YouTube, why, where it is kept and for how long, and how access can be revoked. The Application uses YouTube API Services; by using it you also agree to the [YouTube Terms of Service](https://www.youtube.com/t/terms), and Google's handling of data is described in the [Google Privacy Policy](https://policies.google.com/privacy).

## 1. Data the Application gets

**From the owner's YouTube channel (with the owner's permission, through Google sign-in — OAuth 2.0):**

- the channel's id, title and handle — to check that the Application uploads to the right channel;
- the videos the Application uploads, their ids, titles, privacy status, publishing time and processing status — to show the owner how an upload went;
- captions and thumbnails the Application sets on those videos;
- when the owner allows it: the channel's YouTube Analytics reports (views, watch time, revenue), to show the owner how the channel's videos perform.

The permissions asked for are: `youtube.force-ssl` (upload videos, set thumbnails and captions, edit the channel's own videos), `yt-analytics.readonly` and `yt-analytics-monetary.readonly` (read the channel's analytics). The Application does not read, write or delete anything else in the Google account.

**Public data of other channels (YouTube Data API with an API key, no sign-in):** titles, short descriptions, publishing dates, durations, view, like and comment counts of public videos and the titles and subscriber counts of public channels found by searches the owner runs — to research which topics an audience watches.

The Application does not collect data about any person other than the owner, does not use cookies or tracking, and shows no advertising.

## 2. How the data is used

Only to do what the owner asks the Application to do: research topics, prepare and upload videos to the owner's channel, and show the owner the state of uploads and the channel's results. The data is not sold, not shared with third parties, and not used for advertising or profiling.

To write and check videos the Application sends the owner's own scripts and media to AI model providers (through OpenRouter). Of the data obtained from YouTube API Services, only titles and short descriptions of public videos (as research material) and links to public videos the owner asks to analyse are sent to them; no data of the owner's Google account or channel is sent.

## 3. Where the data is kept

Everything stays on the owner's computer:

- the access grant to the channel (the OAuth refresh token) is kept in Windows Credential Manager of the owner's Windows account; short-lived access tokens are kept in memory only and never written to disk;
- the OAuth client and the API key are kept in a configuration file readable only by the owner's account;
- data about uploads and research results are kept in a local database on the same computer, accessible only to the owner's account.

Nothing is stored on servers of the Application (it has none).

## 4. How long it is kept

- Data obtained from YouTube API Services about other channels' videos and channels (research data) is deleted at the latest 30 days after it was obtained; only the owner's own conclusions (topic ideas, notes) are kept.
- Data about the owner's own channel and uploads is kept while the owner uses the Application; the owner can delete it with the Application's data folder.
- The access grant is kept until the owner disconnects the channel.

## 5. How to revoke access

- In the Application: Profile → «YouTube channel» → «Disconnect channel». The Application revokes the grant at Google and removes it from Windows Credential Manager.
- In the Google account at any time: [https://myaccount.google.com/permissions](https://myaccount.google.com/permissions) → remove "AI Content".

After access is revoked the Application cannot upload or read anything of the channel.

## 6. Security

The Application listens only on the computer's loopback address, accepts connections only from processes of the owner's Windows account, sends tokens and keys only to Google over HTTPS and only in request headers or bodies, and never writes them to logs.

## 7. Changes and contact

Changes to this policy are published at this address with a new date. Questions about this policy: [kyg.hamster@gmail.com](mailto:kyg.hamster@gmail.com).
