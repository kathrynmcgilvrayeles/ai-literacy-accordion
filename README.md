<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>AI Literacy Accordion Activity</title>
    <link href="https://fonts.googleapis.com/css2?family=Open+Sans&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Open Sans', sans-serif;
            background-color: #1f2a52;
            color: #ffffff;
            padding: 20px;
        }
        .accordion {
            background-color: #80dfe3;
            color: #1f2a52;
            cursor: pointer;
            padding: 15px;
            width: 100%;
            border: none;
            text-align: left;
            outline: none;
            font-size: 18px;
            transition: 0.4s;
            margin-top: 5px;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }
        .accordion::after {
            content: '\25BC';
            font-size: 14px;
            color: #1f2a52;
            margin-left: 10px;
        }
        .active::after {
            content: '\25B2';
        }
        .active, .accordion:hover {
            background-color: #009ea5;
        }
        .panel {
            padding: 15px;
            display: none;
            background-color: white;
            color: #1f2a52;
            overflow: hidden;
        }
    </style>
</head>
<body>

    <h2>AI Literacy Accordion Activity</h2>
    
    <button class="accordion">AC Era - After ChatGPT</button>
    <div class="panel">
        <p>The AC era, or "After ChatGPT" era, is a term used to describe the period following the release of OpenAI's ChatGPT in November 2022. It signifies a turning point in how we interact with and utilize artificial intelligence, particularly in the realm of language and information.</p>
    </div>

    <button class="accordion">Chatbots</button>
    <div class="panel">
        <p>A chatbot is a computer program designed to simulate human conversation, often over the internet. It can interact with users through text or voice, providing information, answering questions, or performing tasks.</p>
    </div>

    <button class="accordion">Generative AI</button>
    <div class="panel">
        <p>Generative AI refers to artificial intelligence algorithms (like large language models) that can create new, original content, ranging from text and images to music, code, and even synthetic data, by learning the underlying patterns and structure of existing data.</p>
    </div>

    <button class="accordion">Machine Learning</button>
    <div class="panel">
        <p>Machine learning is a type of artificial intelligence where computers learn from data without explicit programming. For example, a machine learning algorithm can be trained to recognise cats in photos by being shown many examples of cats, or to recommend movies based on your viewing history.</p>
    </div>

    <button class="accordion">Deep Learning</button>
    <div class="panel">
        <p>Advanced machine learning using layered networks for complex tasks like image recognition.</p>
    </div>

    <button class="accordion">Natural Language Processing (NLP)</button>
    <div class="panel">
        <p>AI that enables computers to understand and use human language. Machine Learning (ML): Spam filters learn to identify junk mail.</p>
    </div>

    <button class="accordion">Adaptive Learning</button>
    <div class="panel">
        <p>AI-powered adaptive learning personalises education/lessons and learning, adjusting to each learner's needs and pace like a personal tutor.</p>
    </div>

    <button class="accordion">Hallucinations</button>
    <div class="panel">
        <p>AI sometimes produces a hallucination, which is any inaccurate or misleading output. Here’s an example: Perhaps you tell an AI tool that your sister’s name is Robin. There is also a breed of songbird called a robin. An AI hallucination may be represented as, “Your sister is a songbird.”</p>
    </div>

    <script>
        var acc = document.getElementsByClassName("accordion");
        for (var i = 0; i < acc.length; i++) {
            acc[i].addEventListener("click", function() {
                this.classList.toggle("active");
                var panel = this.nextElementSibling;
                if (panel.style.display === "block") {
                    panel.style.display = "none";
                } else {
                    panel.style.display = "block";
                }
            });
        }
    </script>

</body>
</html>
