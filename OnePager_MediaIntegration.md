# BeatTapper – One-Pager: Media Integration

## 1. Common Uses of Media in Rhythm Games
Rhythm games like *Beat Saber*, *Osu!*, and *Dance Dance Revolution* rely heavily on media to define gameplay and feedback.  
Common media uses include:
- **Audio tracks:** Core to gameplay; beats determine input timing.  
- **Visual cues:** Notes, lane highlights, and particle effects that sync with the music.  
- **Feedback effects:** Sound and light bursts for successful hits or misses.  
- **Background visuals:** Dynamic elements that reflect rhythm intensity or combo streaks.  

Media is not only decorative but essential for conveying rhythm, accuracy, and flow.

---

## 2. Strategies for Integrating Media

### Strategy 1: Embedding Media Locally
Store audio, textures, and animations directly inside the game build.  
**Pros:**  
- Faster access and no need for internet connection.  
- Simpler to package and test; ensures consistent performance.  
**Cons:**  
- Larger file sizes and slower initial load times.  
- Requires new builds to add or change content.  

### Strategy 2: Streaming Media On-Demand
Load songs, textures, or effects dynamically from storage or an online source when needed.  
**Pros:**  
- Reduces memory footprint and allows for new content without updating the app.  
- Enables user-generated or downloadable content (e.g., custom songs).  
**Cons:**  
- Requires careful buffering to avoid lag.  
- Dependent on stable connectivity; may complicate licensing and caching.

---

## 3. Approach for BeatTapper
For **BeatTapper**, I plan to use a **hybrid approach**:
- **Embed core media** (UI sounds, default songs, essential visuals) locally for fast, reliable access.  
- **Stream optional songs or visual packs** from local storage or a lightweight CDN to keep the game size small and flexible.  

This method balances reliability with scalability: it ensures the prototype always works offline, while allowing easy future expansion. Local assets guarantee smooth timing performance, and streaming can support additional content later without major redesign.

---

© 2025 BeatTapper – Elaine Hsu
