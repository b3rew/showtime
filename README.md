# Showtime
This project (continuation) aims to add features on-top of [Mantis-Toboggan](https://github.com/utopiaio/Mantis-Toboggan)

### Features / Improvements
- [X] Own repository and organization - as `Mantis-Toboggan` only targets Edna Mall
- [ ] Add 3D flag for 3D movies (Edna Mall only)
- [ ] Scraping Ethio-Yellow pages for **all** cinema showtimes
- [ ] Connect with ETMDB for Amharic movies (has usage restrictions - should be opt-in)
- [ ] Telegram bot to fix typos (especially on Amharic movies)

```bash
# API interface (public)
$ http GET https://api.io/ # list all cinema showtimes
$ http GET https://api.io/:cinima-name # list specific cinema showtime
$ http GET https://api.io/:cinema-id # list specific cinema showtime via ID (TBD)

# API interface for Telegram Bot (authenticated via Telegram ID)
$ http GET https://api.io/bot # return movie list for today `MOVIE_TITLE`
$ http PUT https://api.io/bot # add / update a correct movie title

# Telegram
/list # return all movie list
MOVIE_TITLE > NEW_MOVIE_TITLE
```

### What it will not have
- Showtime for specific date as database will be flushed to maintain a free-tier

### Stack (Alphabetical Order) - TBD
- Language: Java, Node (current), PHP, Python
- Database: Mongo, MySQL, Postgres (current)
- Platform: AWS, Digital Ocean, Heroku (current), Linode
