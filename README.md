<h1>Fixing No Audio/Dummy Output/No Output Device On All Chromebooks</h1>

<p>Here is a solution to this common issue. This is a simple and fast way to fix audio issues.</p>

<h2>How To Fix</h2>
<h3>1. Download the asound.state file</h3>
<h3>2. Open a terminal and use the following commands (make sure you closed the settings application before doing this)</h3>
<code>sudo cp (downloaded file directory)/asound.state /var/lib/alsa/asound.state/</code>

<code>sudo alsa force-reload alsactl init sudo alsactl store --file /var/lib/alsa/asound.state sudo alsa force-reload</code>
<h3>Done! Open your settings and go to audio and it should say your audio input and output! No need to restart either!</h3>
