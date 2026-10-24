# yoto-callback

Static https page that Yoto's login redirects to; it forwards `code`/`state` to the Audiowissel → Yoto app on the home network (`http://10.10.10.100:8096/auth/yoto/callback`). Needed because Yoto only accepts https callback URLs.

The code is single-use and useless without the PKCE verifier that only the app has.
