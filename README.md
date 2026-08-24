# My resumes

## Running locally

Requires [uv](https://docs.astral.sh/uv/)

```sh
uv sync
uv run rendercv render resumes/english.yaml
uv run rendercv render resumes/portuguese.yaml
```

PDFs are written to `rendercv_output/`. To preview the landing page with the PDFs, copy them into `site/` and open `site/index.html`

## Adding a language

1. Create `resumes/<language>.yaml` with a unique `pdf_path` in `settings.render_command`
2. Add a button in `site/index.html` pointing to that PDF
