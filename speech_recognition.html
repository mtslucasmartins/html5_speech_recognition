<!DOCTYPE html>
<html lang="en">

<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <meta http-equiv="X-UA-Compatible" content="ie=edge">
  <title>Speech Recognition</title>

  <link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css"
    integrity="sha384-MCw98/SFnGE8fJT3GXwEOngsV7Zt27NXFoaoApmYm81iuXoPkFOJwJ8ERdknLPMO" crossorigin="anonymous">

  <script src="https://kit.fontawesome.com/69d1734429.js"></script>

  <style>
    * {
      font-family: "Roboto", "HelveticaNeue-Light""IBM Plex Sans", sans-serif;
      font-weight: 300;
      /* letter-spacing:  */
    }
  </style>

</head>

<body class="w-100 h-100 p-0 m-0 bg-light">
  <div class="border shadow-sm container-fluid px-0 py-3 mx-0 bg-white">
    <header class="container">
      <h4>HTML5 Speech Recognition Example</h4>
    </header>
  </div>
  <div class="container-fluid text-center py-5 mt-5">
    <div class="row">
      <div class="container">
        <h3 id="record-transcription-area"></h3>
      </div>
    </div>
  </div>
  <div class="container-fluid text-center py-0 mt-0">
    <div class="row">
      <div id="sr-alternatives-container" class="container">
        <small class="text-muted mt-2">Alternatives will show here:</small><br>
        <span class="badge badge-primary px-3 py-2">have a nice day</span>
        <span class="badge badge-primary px-3 py-2">I have a nice day</span>
        <span class="badge badge-primary px-3 py-2">having a nice day</span>
        <span class="badge badge-primary px-3 py-2">have a nice.day</span>
      </div>
    </div>
  </div>
  <div class="container-fluid text-center py-5">
    <div class="row">
      <div class="border rounded shadow-sm bg-white container p-4">
        <div class="form-group text-left">
          <label for="exampleInputEmail1">Say something amazing:</label>
          <div class="input-group">
            <input type="text" class="form-control" placeholder="Have a nice day!" aria-label="Recipiente para nickname"
              aria-describedby="basic-addon2">
            <div class="input-group-append">
              <span id="record-toggle" class="input-group-text bg-light text-dark">
                <i id="record-toggle-icon" class="fas fa-microphone-alt"></i>
              </span>
            </div>
          </div>
          <small id="emailHelp" class="form-text text-muted">
            Press the microphone button to the right, and belt out!
          </small>
        </div>

      </div>
    </div>
  </div>
  <script>
    let isRecording = false;

    function setupSpeechRecognition(lang = "pt-BR") {
      let SpeechRecognition = window.SpeechRecognition || window.webkitSpeechRecognition;
      const recognition = new SpeechRecognition();
      recognition.interimResults = true;
      recognition.lang = "en" || lang;
      recognition.continuous = true;
      recognition.maxAlternatives = 5;
      return recognition;
    }

    window.onload = function () {
      const that = this;
      const recordToggleButton = document.querySelector('#record-toggle');
      const recordToggleButtonIcon = document.querySelector('#record-toggle-icon');
      const recordTranscriptionArea = document.querySelector('#record-transcription-area');
      const recognition = this.setupSpeechRecognition();
      recognition.onstart = function () {
        that.isRecording = true;
        that.toggleCssClasses(recordToggleButton, 'bg-success', 'bg-light');
        that.toggleCssClasses(recordToggleButton, 'text-light', 'text-dark');
      };
      recognition.onend = function () {
        that.isRecording = false;
        that.toggleCssClasses(recordToggleButton, 'bg-success', 'bg-light');
        that.toggleCssClasses(recordToggleButton, 'text-light', 'text-dark');
      };
      recognition.onresult = function (event) {
        that.showAlternatives(event);
        transcription = "";
        for (let result of event.results) {
          transcription += result[0].transcript;
        }
        recordTranscriptionArea.innerHTML = transcription;
      };
      recognition.onnomatch = function () {
        transcription = "Oh sorry, I couldn't hear you!";
        recordTranscriptionArea.innerHTML = transcription;
      };
      recordToggleButton.addEventListener('click', function (e) {
        if (that.isRecording) {
          recognition.stop();
          return;
        }
        recognition.start();
      }, false);
    };

    createElement = (name, classes = "", innerHTML = "") => {
      let element = document.createElement(name);
      element.className = classes;
      element.innerHTML = innerHTML;
      return element;
    }

    showAlternatives = (event) => {
      const srAlternativesContainer = document.querySelector('#sr-alternatives-container');
      srAlternativesContainer.innerHTML = '';
      let counter = 0;
      for (let result of event.results) {
        srAlternativesContainer.appendChild(createElement(
          'small', "text-muted mt-2", `Result ${++counter}:`
        ));
        srAlternativesContainer.appendChild(document.createElement('br'));
        for (let alternative of result) {
          srAlternativesContainer.appendChild(createElement(
            'span', "badge badge-primary px-3 py-2 m-2", alternative.transcript
          ));
        }
        srAlternativesContainer.appendChild(document.createElement('br'));
      }
    };

    // CSS Utilities 
    function toggleCssClasses(el, c1, c2) {
      if (containsCssClass(el, c1)) {
        removeCssClass(el, c1);
        appendCssClass(el, c2);
      } else {
        removeCssClass(el, c2);
        appendCssClass(el, c1);
      }
    }
    containsCssClass = (el, c) => el.className.split(" ").indexOf(c) >= 0;
    removeCssClass = (el, c) => {
      let classes = el.className.split(" ");
      classes.splice(classes.indexOf(c), 1);
      el.className = classes.join(" ");
    };
    function appendCssClass(el, c) {
      let classes = el.className.split(" ");
      classes.push(c);
      el.className = classes.join(" ");
    }
  </script>
</body>

</html>