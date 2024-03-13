# ytp

Script for easier download of specific resolutions of videos using [yt-dlp](https://github.com/yt-dlp/yt-dlp).
<br/>
[yt-dlp](https://github.com/yt-dlp/yt-dlp) must be installed and accessible from the PATH in order for this script to work.

## Usage

<code>ytp -p &lt;360/720/1080/...&gt; &lt;url&gt; -o &lt;out.%&gt;</code>

### Parameters

- <p><code>-p &lt;r&gt;</code> download file with height of at most <code>r</code>.<br/>The option can be shortened into just '<code>r</code>p' as shown in the examples.<br/>Without this option the best video resolution is downloaded.<br/>Example values: 360p, 720p, 1080p, ...</p>

- <o><code>-o &lt;path&gt;</code> set path of downloaded file.<br/>All percent characters are replaced by the downloaded file extension.<br/>Example: <code>-o 'file.%'</code> can be downloaded into file <code>file.webm</code>.


### Examples

<code>ytp 360p 'https://www.youtube.com/watch?v=pVGUs9nQGaw' -o 'out.%'</code>
<br/>
Downloads a video from the provided url at a maximum resolution of <code>360p</code> as file <code>out.webm</code>.


<code>ytp 'https://www.youtube.com/watch?v=pVGUs9nQGaw'</code>
<br/>
Downloads a video from the provided url at a maximum possible resolution.