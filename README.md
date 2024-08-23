# Thumbnail Server

A simple web server that displays thumbnails of images.

To run the project move into the project directory and run `sqlx database create` to create the database.
From here you can then `cargo run` the application, the web page will be accessible at [LOCALHOST:3000](http://127.0.0.1:3000/).

## Routes

| Route            | Description                                                            |
| ---------------- | ---------------------------------------------------------------------- |
| `/`              | Display thumbnails of all images. Includes a form for adding an image. |
| `/images`        | JSON list of all uploaded images.                                      |
| [POST] `/upload` | Upload a new image and create a thumbnail.                             |
| `/image/<id>`    | Display a single image.                                                |
| `/thumb/<id>`    | Display a single thumbnail.                                            |
| [POST] `/search` | Find images by tag.                                                    |

> This project demonstrates the learnings from the third week of the [Ardan Labs: Ultimate Rust Foundations](https://www.ardanlabs.com/training/individual-on-demand/rust-bundle/) course.
