# Pixelist Audio Lab hardware tests

Android local test builds can upload queued numeric hardware reports here after the tester configures a repository-scoped GitHub credential on the device. No credential is bundled in the APK or written into reports. No device report has been uploaded until a real phone executes the build and sync is configured.

Reports: `hardware-tests/<random-install-id>/<random-report-id>.json`.

Fields: app version and frozen web bundle SHA-256; random install/report IDs; UTC timestamp; manufacturer/model/SoC, Android SDK, ABI, logical cores, RAM, display size/density, Android WebView version, thermal status when available; sample rate, exposed channel count, panel count, target/observed display FPS, frame p95/p99, numerical JS update cost, FFT size, nominal Web Audio latency, processing-channel counts, pending journal queue peak, measurement duration, source mode and recording-active flag.

Excluded: audio, filenames, project/take names, passwords/tokens, usernames, phone numbers, IMEI/serial/Android ID, contacts, location, IP address and full browser user-agent. Install ID is randomly generated and scoped to the app installation.

These are field-test measurements, not certification of minimum production hardware, acoustic latency, ADC quality, USB compatibility or uninterrupted background recording. Compare matching app bundle, analysis settings and panel/channel counts. Android may defer background synchronization; pending reports remain on the phone until acknowledged by GitHub.
