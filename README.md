# Lampcress 1.0 TEST
Native Android Cocktail Lamp corner-network puzzle. Android 8+ (min26), target35. Package com.gg007.lampcress. Twelve original unique boards on a compact 4x4 grid.

## Rules
Cocktail Lamp on a 4x4 grid with five outlined rooms. Tap individual cells to shade or clear. A gold letter/number label identifies its room and exact shaded-cell total; the label cell may itself be shaded. All shaded cells within a room must form one edge-connected block. Shaded cells across different rooms may not share edges. All room blocks must join into one network through corner contacts. No all-dark 2x2 square. Light cells need not connect. Standard rules allow empty unnumbered rooms; all five rooms in this edition have positive clues. Undo/reset and next/levels; saved palette and optional dark-cell dots. Known Cocktail Lamp adaptation.

## Download and status
https://mega.co.nz/#!ZMVGTSja!n8PHHJQ75rWSb7vEvZgQe2UcodLwAETwNi6jEBK8_8Y
APK SHA256 d681b962a0ad8a35cf63ce099c64bf55951ea054fc5c76cc067893a8b2ca5c81; 16878 bytes. Original signing certificate SHA256 1651d9e269ece8a76f36ed4bba24ebc50f9de1e5f856e0567e0e8169fcb25597. Anonymous downloaded bytes match. No requested permissions. Original icon unchanged.

## Checks
A portable seed-701109 generator checks every 4x4 shading and groups valid candidates by room totals. It selects twelve different five-room layouts, each with exactly one solution and a different completed shading. Independent union-find checks room components and the global corner network, while production uses bit-mask floods. All 786,432 board/mask comparisons agree, including quota counts, cross-border edge exclusion and dark 2x2 rejection. Bounds, individual-cell taps, undo/reset and solved lock pass. Actual drawing-adapter taps solve all twelve and check undo/replay, next, levels, menu, privacy and saved palette/dark marks. Six drawing previews inspected, not phone screenshots. Phone runtime/performance/external-browser QA and full Git source commit remain incomplete. Signed TEST, not final or Play published.

## Functional difference
Reviewed all 201 live studio descriptions and current 803-entry web registry using functional terms. The only cocktail text match was PourMath, a dilution calculator, not a puzzle. No matching room-block corner-network rules in this partial corpus. Isleward also places one dark block per room, but compares adjacent room block sizes and has no global connectivity constraint. Lampcress instead joins all blocks through corners and prohibits dark 2x2 squares, with no unequal-size-neighbor rule. Shapechain uses clue-owned free blocks with no repeated shape in each corner chain, not fixed room quotas. Known Cocktail Lamp adaptation; original generated layouts, code and visuals. No copied layouts/code/art or global invention/history claim. Five fetched base-rule sources agree; a sixth variant article distinguishes its two-block exception, which is not used.
Rules https://www.janko.at/Raetsel/Cocktail-Lampe/index.htm ; independent rules https://www.cross-plus-a.com/html/cros7ctlp.htm .

## Build
JDK17, Android SDK35/build-tools35.0.0. python generate-levels.py reproduces levels.json. javac -d /tmp/blue-test src/com/gg007/lampcress/Board.java BoardTest.java then java -cp /tmp/blue-test com.gg007.lampcress.LampBoardTest. bash build.sh makes an unsigned aligned APK unless KEYSTORE_PATH and KEYSTORE_PASSWORD_FILE point to your own private signing material. No signing secret is included.

## Privacy and branding
Lampcress runs offline without accounts, ads, analytics, third-party SDKs or requested permissions. Palette, dark-cell marks and solved-board marks stay in this app on your device. Clear app data or uninstall to remove them. The studio link opens your external browser.
GG007 original icon, menu studio https://ilanis-agent.github.io/gg-007-gaming/ and privacy.

## Preservation and publishing
Complete source/APK, exact cumulative 202-card studio and published catalog/studio sources and updater privately preserved at https://files.instinct.com/jfrooxqbnqsd-lampcress-source-archive . Repository https://github.com/iLanis-agent/lampcress holds README only; full Git source commit pending. Existing Jekyll static includes retained without changes; no Pages settings changes or client loader. Both site publications verified separately.
