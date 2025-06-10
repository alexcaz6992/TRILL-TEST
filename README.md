# TRILL-TEST

<button onclick="loginWithSpotify()">Log in with Spotify</button>

<script>
  function loginWithSpotify() {
    const client_id = '487ac258fe0c413f942b7e5aa63eab8b';
    const redirect_uri = 'https://trill-test.vercel.app/callback';
    const scope = 'user-read-private user-read-email';
    
    const authUrl = `https://accounts.spotify.com/authorize?response_type=code&client_id=${client_id}&scope=${encodeURIComponent(scope)}&redirect_uri=${encodeURIComponent(redirect_uri)}`;
    
    window.location.href = authUrl;
  }
</script>
