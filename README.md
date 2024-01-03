name: Repositories and diff history
uses: lowlighter/metrics@latest
with:
  filename: metrics.plugin.lines.history.svg
  token: ${{ secrets.METRICS_TOKEN }}
  base: ""
  plugin_lines: yes
  plugin_lines_delay: 30
  plugin_lines_sections: repositories, history
  plugin_lines_repositories_limit: 2
  plugin_lines_history_limit: 1
  repositories_skipped: |
    @use.patterns
    */*
    +lowlighter/metrics
