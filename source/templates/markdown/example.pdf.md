# Open Source Resume
**Powered by [lowlighter/metrics](https://github.com/lowlighter/metrics)**

<%- await include(`partials/rss.ejs`) %>

## Basic info
<%- await embed(
  `resume-template`, 
  {
    base: ['header', 'activity', 'community', 'repositories', 'metadata'],
    repositories_forks: true,
    plugin_followup: false,
    plugin_notable: true,
    plugin_lines: true,
    plugin_isocalendar: true,
    plugin_languages: true,
    plugin_stackoverflow: 1674992,
    plugin_stackoverflow_limit: 3,
    plugin_stackoverflow_lines: 4
    plugin_isocalendar_duration: 'full-year',
    plugin_stackoverflow_sections: ['answers-top', 'answers-recent'],
  }
) %>