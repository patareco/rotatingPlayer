# rotatingYTPlayer

A simple custom youtube player that change orientation for videos that are both vertical and horizontal. The target usage is mainly on desktop since most user can't easily rotate their screen.

Demo: https://nchantre.com/wp/wp-content/experiments/drone.html

## dynamic URL loading

The player assumes a 9:16 aspect ratio. Will implement more options in the future.

### URL Params

- id: Youtube Video ID
- r: comma separated moments of rotation with the following structure: degrees@timecode+duration

The degrees have to have a 'deg' suffix since the value is injected directly in CSS.
The duration has to have an 's' suffix.

### Example

full url:
rotatingYTPlayer.html?id=IUMTaAQ43lY&r=-90deg@20+2s,0deg@40+0.5s,-180deg@60+5s,-90deg@90+5s,-90deg@120+2s

### Using with iframe

```xml
<!-- 9/16 aspect ratio with vh units -->
<iframe src="https://gitcdn.xyz/repo/patareco/rotatingYTPlayer/master/rotatingYTPlayer.html?id=ydvik6N0Igc&r=-90deg@46+2s,-270deg@81+2s,-90deg@88+1s" width="50.5vh" height="90vh"></iframe>
```