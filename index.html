<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Drag and Drop Sentence Order</title>
  <style>
    body { font-family: Arial, sans-serif; padding: 20px; }
    .question { margin-bottom: 40px; }
    .drop-zone, .choices { border: 2px dashed #ccc; padding: 10px; min-height: 50px; display: flex; flex-wrap: wrap; gap: 8px; margin-bottom: 10px; }
    .word { padding: 8px 12px; background: #f0f0f0; border: 1px solid #ccc; border-radius: 8px; cursor: move; user-select: none; }
    .check-btn, .reset-btn, .shuffle-btn { margin-top: 10px; padding: 6px 12px; border: none; color: white; border-radius: 5px; cursor: pointer; margin-right: 10px; }
    .check-btn { background-color: #4CAF50; }
    .reset-btn { background-color: #f44336; }
    .shuffle-btn { background-color: #2196F3; }
    .result { margin-top: 8px; font-weight: bold; }
    .correct { color: green; }
    .incorrect { color: red; }
    h3 { margin-bottom: 10px; }
  </style>
</head>
<body>
  <button class="shuffle-btn" onclick="shuffleQuestions(true)">🔀 Shuffle Questions</button>
  <div id="questions-container"></div>

  <script>
    function shuffleArray(array) {
      const arr = array.slice();
      for (let i = arr.length - 1; i > 0; i--) {
        const j = Math.floor(Math.random() * (i + 1));
        [arr[i], arr[j]] = [arr[j], arr[i]];
      }
      return arr;
    }

     const questions = [
      { id: 1, title: "Question 1", words: ["Children", "shouldn’t", "see", "that film", "because", "its content", "is", "too violent."], correct: ["Children", "shouldn’t", "see", "that film", "because", "its content", "is", "too violent."] },
      { id: 2, title: "Question 2", words: ["Spider Man films", "were", "produced", "in", "the USA", "by", "Columbia Pictures."], correct: ["Spider Man films", "were", "produced", "in", "the USA", "by", "Columbia Pictures."] },
      { id: 3, title: "Question 3", words: ["I", "don’t", "have", "enough", "information", "to", "finish", "my report", "before", "Friday."], correct: ["I", "don’t", "have", "enough", "information", "to", "finish", "my report", "before", "Friday."] },
      { id: 4, title: "Question 4", words: ["What movie", "did", "you", "want", "to", "watch again", "as soon as", "it", "finished?"], correct: ["What movie", "did", "you", "want", "to", "watch again", "as soon as", "it", "finished?"] },
      { id: 5, title: "Question 5", words: ["Serena", "was", "watching", "a", "romantic film", "when", "the power", "went", "out."], correct: ["Serena", "was", "watching", "a", "romantic film", "when", "the power", "went", "out."] },
      { id: 6, title: "Question 6", words: ["Radios", "were", "used", "to", "give", "important news", "during", "the second", "World War."], correct: ["Radios", "were", "used", "to", "give", "important news", "during", "the second", "World War."] },
      { id: 7, title: "Question 7", words: ["The keyboard", "was", "made of", "plastic, so", "it’s light", "and easy", "to carry."], correct: ["The keyboard", "was", "made of", "plastic, so", "it’s light", "and easy", "to carry."] },
      { id: 8, title: "Question 8", words: ["In the 1440s,", "the first", "printing press", "was invented", "and it", "could print", "many books", "quickly."], correct: ["In the 1440s,", "the first", "printing press", "was invented", "and it", "could print", "many books", "quickly."] },
      { id: 9, title: "Question 9", words: ["Was", "the", "first", "video game", "created", "in", "the 1950s?"], correct: ["Was", "the", "first", "video game", "created", "in", "the 1950s?"] },
      { id: 10, title: "Question 10", words: ["In the past,", "phones", "were", "used mainly", "for making", "calls and", "sending simple", "text messages."], correct: ["In the past,", "phones", "were", "used mainly", "for making", "calls and", "sending simple", "text messages."] },
      { id: 11, title: "Question 11", words: ["on social media", "Photos of", "free-time activities", "by", "every day", "shared", "are", "Tom."], correct: ["Photos of", "free-time activities", "are", "shared", "on social media", "every day", "by", "Tom."] },
      { id: 12, title: "Question 12", words: ["What", "for", "to", "information?", "search", "you", "do", "use", "tools"], correct: ["What", "tools", "do", "you", "use", "to", "search", "for", "information?"] },
      { id: 13, title: "Question 13", words: ["is", "after ten minutes", "usually", "save", "to", "battery power.", "The screen", "turned off"], correct: ["The screen", "is", "usually", "turned off", "after ten minutes", "to", "save", "battery power."] },
      { id: 14, title: "Question 14", words: ["How", "saved", "on", "important information", "is", "your computer?"], correct: ["How", "is", "important information", "saved", "on", "your computer?"] },
      { id: 15, title: "Question 15", words: ["or actors", "you", "singers", "follow", "famous", "any", "Do", "Instagram?", "on"], correct: ["Do", "you", "follow", "any", "famous", "singers", "or actors", "on", "Instagram?"] },
      { id: 16, title: "Question 16", words: ["to play", "a musical", "instrument", "to learn", "a good", "be", "or piano.", "like guitar", "It would", "idea"], correct: ["It would", "be", "a good", "idea", "to learn", "to play", "a musical", "instrument", "like guitar", "or piano."] },
      { id: 17, title: "Question 17", words: ["think", "be", "it would", "a live", "Do you", "Korean concert", "great", "to attend", "by Black Pink?"], correct: ["Do you", "think", "it would", "be", "great", "to attend", "a live", "Korean concert", "by Black Pink?"] },
      { id: 18, title: "Question 18", words: ["in", "play football", "at school.", "when", "were", "we", "students", "We'd", "football ground"], correct: ["We'd", "play football", "in", "football ground", "when", "we", "were", "students", "at school."] },
      { id: 19, title: "Question 19", words: ["have", "to travel", "enough money", "we would", "competition,", "If we", "to Thailand.", "this sports", "won"], correct: ["If we", "won", "this sports", "competition,", "we would", "have", "enough money", "to travel", "to Thailand."] },
      { id: 20, title: "Question 20", words: ["the afternoon.", "wouldn't", "at noon,", "often sleep", "in", "My father", "really tired", "he felt", "so"], correct: ["My father", "wouldn't", "often sleep", "at noon,", "so", "he felt", "really tired", "in", "the afternoon."] },
      { id: 21, title: "Question 21", words: ["it’s", "because", "too", "horse racing", "go", "for", "cannot", "She", "her.", "expensive"], correct: ["She", "cannot", "go", "horse racing", "because", "it’s", "too", "expensive", "for", "her."] },
      { id: 22, title: "Question 22", words: ["must", "to", "fit and", "They", "them", "stay", "do", "keep", "healthy.", "judo"], correct: ["They", "must", "do", "judo", "to", "stay", "fit and", "keep", "them", "healthy."] },
      { id: 23, title: "Question 23", words: ["you", "can", "kind", "musical", "play?", "What", "instrument", "of"], correct: ["What", "kind", "of", "musical", "instrument", "can", "you", "play?"] },
      { id: 24, title: "Question 24", words: ["the", "sporting", "events?", "Why", "we", "organize", "have to", "do"], correct: ["Why", "do", "we", "have to", "organize", "the", "sporting", "events?"] },
      { id: 25, title: "Question 25", words: ["play", "you", "could", "What sport", "at", "you", "high school?", "when", "were"], correct: ["What sport", "could", "you", "play", "when", "you", "were", "at", "high school?"] },
      { id: 26, title: "Question 26", words: ["they couldn’t", "but", "get tickets.", "went to", "the theatre,", "They"], correct: ["They", "went to", "the theatre,", "but", "they couldn’t", "get tickets."] },
      { id: 27, title: "Question 27", words: ["The", "were really", "arrived at", "when they", "tourists", "tired", "the hotel."], correct: ["The tourists", "were really", "tired", "when they", "arrived at", "the hotel."] },
      { id: 28, title: "Question 28", words: ["were exploring", "and Sarah", "when", "got lost.", "John", "the island", "they suddenly"], correct: ["John", "and Sarah", "were exploring", "the island", "when", "they suddenly", "got lost."] },
      { id: 29, title: "Question 29", words: ["a great time", "while they", "to visit", "were there.", "The group", "was having", "Paris"], correct: ["The group", "was having", "a great time", "while they", "were there", "to visit", "Paris."] },
      { id: 30, title: "Question 30", words: ["sightseeing", "was going", "yesterday.", "the city", "all day", "She", "in"], correct: ["She", "was going", "sightseeing", "in", "the city", "all day", "yesterday."] },
       { id: 31, title: "Question 31", words: ["yesterday.", "in the town", "the museum", "We", "visited"], correct: ["We", "visited", "the museum", "in the town", "yesterday."] },
      { id: 32, title: "Question 32", words: ["the accident.", "Linda", "when", "she", "saw", "the guidebook", "was reading"], correct: ["Linda", "was reading", "the guidebook", "when", "she", "saw", "the accident."] },
      { id: 33, title: "Question 33", words: ["The", "across the mountains.", "to take", "Korean tourists", "hired", "a local guide", "them"], correct: ["The", "Korean tourists", "hired", "a local guide", "to take", "them", "across the mountains."] },
      { id: 34, title: "Question 34", words: ["I", "every ten years", "a new passport", "changes.", "my face", "need to", "because", "get"], correct: ["I", "need to", "get", "a new passport", "every ten years", "because", "my face", "changes."] },
      { id: 35, title: "Question 35", words: ["were", "taking photos", "it started", "when", "to rain.", "They"], correct: ["They", "were", "taking photos", "when", "it started", "to rain."] },
      { id: 36, title: "Question 36", words: ["Marre", "when", "her", "homework", "she", "got", "did", "from the zoo.", "home"], correct: ["Marre", "did", "her", "homework", "when", "she", "got", "home", "from the zoo."] },
      { id: 37, title: "Question 37", words: ["my computer.", "I", "some", "animals", "photographs", "like", "in", "taking", "to", "of", "save"], correct: ["I", "like", "taking", "photographs", "of", "some", "animals", "to", "save", "in", "my computer."] },
      { id: 38, title: "Question 38", words: ["It", "for", "to", "London.", "to", "buses", "move", "is", "school", "difficult"], correct: ["It", "is", "difficult", "for", "school", "buses", "to", "move", "to", "London."] },
      { id: 39, title: "Question 39", words: ["at", "sister", "playing", "My", "guitar.", "is", "good", "really", "the"], correct: ["My", "sister", "is", "really", "good", "at", "playing", "the", "guitar."] },
      { id: 40, title: "Question 40", words: ["to", "enjoy", "going", "on", "my", "the", "own.", "cinema", "I", "don’t"], correct: ["I", "don’t", "enjoy", "going", "to", "the", "cinema", "on", "my", "own."] },
      { id: 41, title: "Question 41", words: ["country?", "of", "in", "What", "mean", "is", "the", "most", "popular", "your", "transport"], correct: ["What", "is", "the", "most", "popular", "mean", "of", "transport", "in", "your", "country?"] },
      { id: 42, title: "Question 42", words: ["better", "Which", "do", "place", "is", "live?", "to", "you", "think"], correct: ["Which", "place", "do", "you", "think", "is", "better", "to", "live?"] },
      { id: 43, title: "Question 43", words: ["bicycles", "every day.", "school", "often", "students", "ride", "Young", "to"], correct: ["Young", "students", "often", "ride", "bicycles", "to", "school", "every day."] },
      { id: 44, title: "Question 44", words: ["busy", "to", "was", "to", "him", "take", "too", "Peter's mother", "the cinema."], correct: ["Peter's mother", "was", "too", "busy", "to", "take", "him", "to", "the cinema."] },
      { id: 45, title: "Question 45", words: ["download", "fast", "the", "enough", "film.", "to", "The laptop", "isn't"], correct: ["The laptop", "isn't", "fast", "enough", "to", "download", "the", "film."] }
    ];


    const originalWords = {};
    const correctAnswers = {};

    function createQuestionHTML(q, index) {
      const container = document.createElement('div');
      container.className = 'question';
      container.setAttribute('data-id', q.id);
      container.innerHTML = `
        <h3>Question ${q.id}</h3>
        <div class="drop-zone" id="dropZone${q.id}"></div>
        <div class="choices" id="choices${q.id}"></div>
        <button class="check-btn" onclick="checkAnswer(${q.id})">Check Answer</button>
        <button class="reset-btn" onclick="resetQuestion(${q.id})">Reset</button>
        <div id="result${q.id}" class="result"></div>
      `;
      document.getElementById('questions-container').appendChild(container);

      const dropZone = container.querySelector(`#dropZone${q.id}`);
      const choices = container.querySelector(`#choices${q.id}`);
      const shuffled = shuffleArray(q.words);
      shuffled.forEach(text => {
        const word = document.createElement('div');
        word.className = 'word';
        word.draggable = true;
        word.textContent = text;
        choices.appendChild(word);
      });
    }

    function renderQuestions() {
      document.getElementById('questions-container').innerHTML = '';
      questions.forEach(q => {
        originalWords[q.id] = q.words;
        correctAnswers[q.id] = q.correct;
        createQuestionHTML(q);
      });
      enableDragEvents();
      setupDropZones();
    }

    function shuffleQuestions(resetWords = false) {
      const shuffledQuestions = shuffleArray(questions);
      document.getElementById('questions-container').innerHTML = '';
      shuffledQuestions.forEach(q => {
        if (resetWords) {
          originalWords[q.id] = q.words;
          correctAnswers[q.id] = q.correct;
        }
        createQuestionHTML(q);
      });
      enableDragEvents();
      setupDropZones();
    }

    let draggedItem = null;

    function enableDragEvents() {
      document.querySelectorAll('.word').forEach(word => {
        word.addEventListener('dragstart', () => draggedItem = word);
        word.addEventListener('dragend', () => draggedItem = null);
      });
    }

    function resetQuestion(questionNum) {
      const dropZone = document.getElementById(`dropZone${questionNum}`);
      const choices = document.getElementById(`choices${questionNum}`);
      const resultBox = document.getElementById(`result${questionNum}`);
      dropZone.innerHTML = '';
      choices.innerHTML = '';
      const shuffled = shuffleArray(originalWords[questionNum]);
      shuffled.forEach(text => {
        const word = document.createElement('div');
        word.className = 'word';
        word.draggable = true;
        word.textContent = text;
        choices.appendChild(word);
      });
      resultBox.textContent = '';
      enableDragEvents();
    }

    function checkAnswer(questionNum) {
      const dropZone = document.getElementById(`dropZone${questionNum}`);
      const resultBox = document.getElementById(`result${questionNum}`);
      const droppedWords = Array.from(dropZone.children).map(word => word.textContent.trim());
      const correctOrder = correctAnswers[questionNum];
      const isCorrect = JSON.stringify(droppedWords) === JSON.stringify(correctOrder);
      resultBox.textContent = isCorrect ? '✅ Correct!' : '❌ Try again.';
      resultBox.className = isCorrect ? 'result correct' : 'result incorrect';
    }

    function setupDropZones() {
      document.querySelectorAll('.drop-zone, .choices').forEach(zone => {
        zone.addEventListener('dragover', e => e.preventDefault());
        zone.addEventListener('drop', e => {
          e.preventDefault();
          if (draggedItem && zone !== draggedItem.parentNode) {
            zone.appendChild(draggedItem);
          }
        });
      });
    }

    renderQuestions();
  </script>
</body>
</html>
