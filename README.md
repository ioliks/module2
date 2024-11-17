module2-solution/
├── index.html
└── css/
    └── styles.css
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Responsive Page</title>
    <link rel="stylesheet" href="css/styles.css">
</head>
<body>
    <header>
        <h1>Responsive Page</h1>
    </header>
    <main>
        <section class="section section-chicken">
            <div class="title">Chicken</div>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam auctor lacus et dolor facilisis.</p>
        </section>
        <section class="section section-beef">
            <div class="title">Beef</div>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam auctor lacus et dolor facilisis.</p>
        </section>
        <section class="section section-sushi">
            <div class="title">Sushi</div>
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nullam auctor lacus et dolor facilisis.</p>
        </section>
    </main>
</body>
</html>


 {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, sans-serif;
    line-height: 1.6;
    margin: 20px;
}


header {
    text-align: center;
    margin-bottom: 20px;
}

header h1 {
    font-size: 2rem;
    color: #333;
}


.section {
    border: 1px solid black;
    padding: 20px;
    margin: 10px;
    position: relative;
    background-color: #f4f4f4;
}

.section .title {
    position: absolute;
    top: 10px;
    right: 10px;
    background-color: #ffdd57;
    color: black;
    padding: 5px;
    border: 1px solid black;
}


.section-chicken {
    background-color: #ffefdb;
}

.section-beef {
    background-color: #fddede;
}

.section-sushi {
    background-color: #dff6ff;
}

/* Media Queries */


@media (min-width: 992px) {
    main {
        display: flex;
        justify-content: space-between;
    }

    .section {
        flex: 1;
        margin: 10px;
    }
}


@media (min-width: 768px) and (max-width: 991px) {
    main {
        display: flex;
        flex-wrap: wrap;
    }

    .section {
        width: 48%;
        margin: 1%;
    }

    .section-sushi {
        width: 100%;
    }
}
@media (max-width: 767px) {
    .section {
        width: 100%;
        margin: 10px 0;
    }
}
@media (max-width: 767px) {
    .section {
        width: 100%;
        margin: 10px 0;
    }
}
