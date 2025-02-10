# Birthday Paradox Game

## Overview

The Birthday Paradox Game is a web-based game built for educational purposes. It leverages the surprising probability phenomenon known as the **Birthday Paradox**—which states that in a group of just 23 people, there is about a 50% chance that two individuals share the same birthday. As the number of people increases, this probability grows dramatically (over 99% with 46 people).

In this game, one user acts as the host to create a game room with a unique 6-character hexadecimal code (displayed in uppercase), and other players can join using that code along with their nickname and birthday (entered in MM-DD format). The game then matches players who share the same birthday.

## Features

- **Game Room Creation:**  
  The host creates a game room with a randomly generated 6-character hexadecimal code. This code is always shown in uppercase, even if a player joins with a lowercase input.

- **Join Game:**  
  Players can join a game by entering the game code, their nickname, and their birthday (in MM-DD format). The game accepts the code in any case but always displays it in uppercase.

- **Real-Time Updates:**  
  The game page updates in real-time, displaying the current player count and room details.

- **Game Control:**  
  The host can end the game. A countdown is triggered, after which the matching results (players sharing the same birthday) are revealed.

- **Informative Section:**  
  An expandable section titled "What is birthday paradox?" provides a concise explanation of the paradox in clear, easy-to-understand English.

- **Responsive & Themed Design:**  
  The interface features a modern, responsive design with a custom "Birthday Paradox" theme, including a gradient background and custom fonts (Google Fonts: Bangers and Roboto). This ensures an enjoyable experience on both desktop and mobile devices.

- **Session Management:**  
  Sensitive data (such as game code and user details) is stored in sessionStorage instead of URL parameters to enhance privacy.

- **Security Measures:**  
  - **Prepared Statements:** All database queries are handled using PDO prepared statements.
  - **Native Prepared Statements:** Emulated prepares are disabled (`PDO::ATTR_EMULATE_PREPARES` set to false) to further reduce SQL injection risks.
  - **Input Validation:** User inputs are validated and sanitized to help prevent common attacks.
  - **Protected Configuration:** Sensitive files (e.g., `config.php`) are protected from direct web access.

## Technologies Used

- **Frontend:** HTML5, CSS3, JavaScript  
- **Backend:** PHP (using PDO for MySQL database interactions)  
- **Database:** MySQL  
- **Additional Tools:**  
  - Code minification and obfuscation techniques are applied to optimize and slightly obscure client-side code.

## Try yourself

ahsdev.com.tr/birthdayparadox
