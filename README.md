# NBA_Stat_Scraper
Scrapes www.basketball-reference.com for NBA player stats.

Uses requests and BeautifulSoup modules to search the site for all players. Asks for player name, and returns table 
of any player with name on the site. 

Program scrapes main (featured) stats from website into lists, and puts them into corresponding distionaries which are later used to create the printed tables.

Table returned is similiar to the one on www.basketball-reference.com. For current players, you get current year and carrer stats. For any other player, you get career stats. It also prints the full name and NBA debut date for each player. 

If no player is found, program returns 'Player not found'. This can occur if spelling of player's name is not correct or it's not the name he uses. The name entered has to match the name on website database. Nicknames probably won't work.

For players with the same name, both tables will be returned. the program prints an "NBA Debut" date for distinction. For this part, the re module was used. Using findAll() function in BeautifulSoup was useful for getting "NBA Debut:" string but the actual date was found using regular expressi

The get_connection function was written to see if www.basketball-reference.com allows web crawling on their site. Not part of actual main() function.
