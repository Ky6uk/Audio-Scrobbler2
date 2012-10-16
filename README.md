[![Build Status](https://travis-ci.org/Ky6uk/Audio-Scrobbler2.png)](https://travis-ci.org/Ky6uk/Audio-Scrobbler2)

# Audio::Scrobbler2 - Interface to last.fm scrobbler API

## Synopsis
```perl
use Audio::Scrobbler2;

my $scrobbler = Audio::Scrobbler2->new($api_key, $api_secret);
my $api_token = $scrobbler->auth_getToken();

# web-auth required
# http://www.last.fm/api/auth/?api_key=$api_key&token=$api_token
my $api_session = $scrobbler->auth_getSession();

$scrobbler->track_scrobble("Artist Name", "Track Name");
```
