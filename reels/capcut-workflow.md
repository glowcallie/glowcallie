# Claude x CapCut 릴스 편집 워크플로

원본은 16:9 유튜브 브이로그 편집 과정이에요.
릴스(9:16)에 맞게 바꿔서 정리했어요.
편집 톤과 자막 기준은 `reels/editing-guide.md`를 함께 따라요.

핵심 방식:
Claude가 CapCut 앱을 직접 조작하지 않아요.
맥에 있는 프로젝트 파일(`draft_content.json`)을 직접 수정해요.
마지막 디테일은 CapCut에서 직접 다듬어요.

결과: 편집 시간 7~8시간 → 1~2시간 (브이로그 기준)

---

## Step 1. 영상 불러오기
1. CapCut을 켜고 촬영한 영상을 모두 불러와요.
2. 화면 비율은 **9:16**으로 설정해요.
3. 프로젝트 이름을 정해요. 예: `Reels_1114`
4. **CapCut 창을 완전히 닫아요.** (열려 있으면 파일 수정이 덮어써져요)

## Step 2. BGM 폴더 만들기
- 바탕화면에 `BGM` 폴더를 만들고 쓸 음원을 넣어요.
- 저작권 걱정 없는 음원을 써요. 예: Epidemic Sound
- 릴스는 비트가 분명한 곡이 컷 전환에 유리해요.

## Step 3. Claude로 편집하기
- **맥에서 파일에 접근할 수 있는 Claude**(Claude 데스크톱 + 파일 접근)에서 진행해요.
- 아래 프롬프트를 붙여넣고, 프로젝트 이름만 바꿔요.
- 레퍼런스 릴스 영상을 함께 첨부해요.
- 자막 폰트, 색상, 자간까지 구체적으로 적을수록 결과가 좋아요.

### 📋 릴스용 프롬프트
```
Hi Claude, please edit my CapCut project "Reels_1114" into a 9:16 Instagram Reel (target 30–60 seconds).

Tasks:
1. Cut out repeats, mistakes, long pauses, and anything out of place. Speed up similar repeated scenes.
2. First 3 seconds: show the title "<제목>" large and centered with a light pop-up animation, and a slow zoom-in on the key result shot.
3. Every 2–3 seconds, add a small change: zoom-in, zoom-out, close-up, or a subtitle change. Avoid flashy transitions.
4. Emphasize key scenes (e.g. scalp check, EMS, ampoule care) with close-ups so details are clear.
5. Cut on the beat of the background music from my "BGM" folder on the Desktop.
6. Add an adjustment layer with slightly boosted saturation and contrast, and lowered shadows.
7. Add Korean subtitles timed to the audio. Step captions (STEP 1, 2, 3) get a light entrance animation. Make key words bigger or bolder.
8. Write info captions in a personal, experience-based tone (e.g. "40대부터는 모발뿐 아니라 두피 상태도 중요하더라고요.").
9. Make the final result shot stand out, and end with a closing caption like "<마무리 다짐 문구> ♡".
10. Overall mood: natural and refined, not flashy. Keep the original natural feel, just more lively.
11. Use the attached reference video for pacing, cut rhythm, subtitle style (font, size, position, color), and mood.
12. Make sure all generated assets use a format and file path CapCut can read.

Constraints:
- Do NOT use computer use or open CapCut. Edit the project files directly through file access on my Mac.
- Back up the original project folder before making any changes.

Before you start:
- Ask me any questions you need to confirm details first.
```

## Step 4. 직접 마무리하기
- CapCut을 다시 열어 결과를 확인해요.
- 자막 위치가 인스타 UI(하단 캡션, 오른쪽 버튼)에 가리지 않는지 확인해요.
- 마지막 디테일은 직접 다듬어요.
