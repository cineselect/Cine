<!DOCTYPE html>
<html>
<head>
	<title>CineSecret</title>
	<style>
		body {
			margin: 0;
			padding: 0;
			background-color: #808080;
			position: relative;
		}

		body::before {
			content: "";
			position: absolute;
			top: 0;
			left: 0;
			width: 100%;
			height: 2cm;
			background-color: black;
		}

		.container {
			display: flex;
			flex-direction: column;
			align-items: center;
			justify-content: center;
			height: 100vh;
		}

		h1 {
			font-size: 8rem;
			font-weight: bold;
			color: white;
			margin: 0;
			padding: 1cm 0 0 0;
			text-align: center;
			line-height: 1;
		}

		button {
			padding: 20px;
			margin-top: 20px;
			background-color: #007bff;
			color: white;
			border: none;
			border-radius: 5px;
			font-size: 1.5rem;
			cursor: pointer;
		}

		p {
			font-size: 2.5rem;
			color: white;
			margin-bottom: 20px;
		}
		
		#title {
			position: absolute;
			top: 0;
			left: 50%;
			transform: translateX(-50%);
			height: 2cm;
			line-height: 2cm;
			font-size: 2rem;
			font-weight: bold;
			color: white;
		}
	</style>
	<script>
		
		function showRandomMovie() {
			var movies = [
				"Iron Man (2008)",
                                "Der unglaubliche Hulk (2008)",
                                "Iron Man 2 (2010)",
                                "Thor (2011) ",
                                "Captain America: The First Avenger (2011)",
                                "Marvel's The Avengers (2012)",
                                "Iron Man 3 (2013)",
                                "Thor: The Dark Kingdom (2013)",
                                "The Return of the First Avenger (2014)",
                                "Guardians of the Galaxy (2014)",
                                "Avengers: Age of Ultron (2015)",
                                "Ant-Man (2015)",
                                "The First Avenger: Civil War (2016)",
                                "Guardians of the Galaxy Vol. 2 (2017)",
                                "Spider-Man: Homecoming (2017)",
                                "Thor: Tag der Entscheidung (2017)",
                                "Black Panther (2018)",
                                "Avengers: Infinity War ",
                                "Ant-Man and the Wasp (2018)",
                                "Captain Marvel (2019)",
                                "Avengers:Endgame (2019)",
                                "Spider-Man: Far From Home (2019)",
                                "WandaVision (2021 bei Disney+)",
                                "The Falcon and the Winter Soldier (2021 bei Disney+)",
                                "Loki (seit 2021 bei Disney+)",
                                "What If...? (seit 2021 bei Disney+)",
                                "Black Widow (2021)",
                                "Shang-Chi and the Legend of the Ten Rings (2021)",
                                "Eternals (2021)",
                                "Hawkeye (2021 bei Disney+)",
                                "Spider-Man: No Way Home (2021)",
                                "Moon Knight (seit 2022 bei Disney+)",
                                "Doctor Strange in the Multiverse of Madness (2022)",
                                "Ms. Marvel (seit 2022 bei Disney+)",
				"Thor: Love and Thunder (2022)",
				"Ich bin Groot (seit 2022 bei Disney+)",
				"She-Hulk: Die Anwältin (seit 2022 bei Disney+)",
				"Black Panther: Wakanda Forever (ab 2022)",
				"Spider man 1 mit T.M",
                                "Spider man 2 mit T.M",
                                "Spider man 3 mit T.M",
                                "Amazing Spider man 1",  
                                "Amazing Spider man 2", 
                                "Star Wars: Episode I - Die dunkle Bedrohung",
                                "Star Wars: Episode II - Angriff der Klonkrieger",
                                "Star Wars: Episode III - Die Rache der Sith",
                                "Rogue One: A Star Wars Story",
                                "Solo: A Star Wars Story",
                                "Star Wars: Episode IV - Eine neue Hoffnung",
                                "Star Wars: Episode V - Das Imperium schlägt zurück",
                                "Star Wars: Episode VI - Die Rückkehr der Jedi-Ritter",
                                "Star Wars: Episode VII - Das Erwachen der Macht",
                                "Star Wars: Episode VIII - Die letzten Jedi",
                                "Star Wars: Episode IX - Der Aufstieg Skywalkers",
                                "Der Hobbit: Eine unerwartete Reise",
                                "Der Hobbit: Smaugs Einöde",
                                "Der Hobbit: Die Schlacht der Fünf Heere",
                                "Der Herr der Ringe: Die Gefährten",
                                "Der Herr der Ringe: Die zwei Türme",
                                "Der Herr der Ringe: Die Rückkehr des Königs",
                                "James BondCasino Royale",
                                "James BondEin Quantum Trost",
                                "James BondSkyfall",
                                "James BondSpectre",
                                "James BondKeine Zeit zu sterben",
                                "Ant-Man and the Wasp: Quantumania (ab 2023)"
			];
			var randomMovie = movies[Math.floor(Math.random() * movies.length)];
			alert(randomMovie);
		}
	</script>
</head>
<body>
	<div id="title">Lu-Colin's Masterwork</div>
	<div class="container">
		<h1>CineSecret</h1>
		<p>Klicke auf den Button, um einen zufälligen Film zu sehen:</p>
		<button onclick="showRandomMovie()">Zufälligen Film anzeigen</button>
	</div>
</body>
</html>
