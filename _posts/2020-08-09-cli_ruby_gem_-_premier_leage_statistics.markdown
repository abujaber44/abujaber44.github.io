---
layout: post
title:      "CLI Ruby Gem - Premier Leage Statistics "
date:       2020-08-09 04:20:33 +0000
permalink:  cli_ruby_gem_-_premier_leage_statistics
---



I had several ideas in mind for this project. The goal is to build something interesting while making sure all the technical requirements are fulfilled. My passion for sports and specifically European soccer had made the choice for me. I decided to build a Ruby Gem that provides statistics for the Premier League players. This CLI project has to be composed of an Object-Oriented Ruby application. One of the requirements is to use a remote source (an API or scrape a website). I decided to build my application using an API.    

*My Ruby Gem provides:*

  1.	A CLI with an interface that users can interact with
  2.	Retrieve data from an API: “https://apifootball.com/” 
  3.	Provides three levels of data. 
      •	 First, the CLI instructs the user to choose a team or list all available teams to choose from. 
      •	Second, the user will select a team, and the CLI will display three options to select from: Top Scorer,        Oldest/Youngest Player, and Display all stats for a specific player. 
     •	Third, the user can select one of the choices mentioned previously to view the requested information. If the choice   is Display all stats for a specific player, then the user will type a player’s name or list all players to choose from. 
 4.	The CLI app has the following files:
     •	CLI.rb: it contains the code handling CLI display logic and user input
     •	Team.rb: it contains the code that initializes the team object based on specific attributes (ID, Name, and Players) 
     •	APIService.rb: it contains the code responsible for retrieving data for the API
     •	environment.rb: it defines all files dependencies 
		 
The program instructs the user to type a team name or list all teams to choose one. The user’s input is interpreted to a team ID since the API endpoint provide information by team ID. The APIService.rb file is responsible for retrieving the data based on the team ID. The Team.rb file will initialize the team with three attributes: ID, name, and players. In the team menu the user can view the top scorer, youngest player, oldest player, or display all stats for a specific player. To view all information for one player, the user needs to type a player name or list all players to choose from. This option will show the following information: player key, player name, player number, player country, player type, player age, player match played, player goals, player yellow cards, and player red cards.



