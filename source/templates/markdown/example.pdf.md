# Open Source Resume
**Powered by [lowlighter/metrics](https://github.com/lowlighter/metrics)**

<%- await include(`partials/rss.ejs`) %>

## Basic info
<%- await embed(
  `resume-template`, 
  {
    isocalendar: true,
    isocalendar_duration: 'full-year',
    base: ['header', 'activity', 'community', 'repositories', 'metadata'],
    stackoverflow_sections: ['answers-top', 'answers-recent'],
    stackoverflow: true,
    stackoverflow_user: 1674992,
    stackoverflow_limit: 3,
    stackoverflow_lines: 4,
    repositories_forks: true,
    followup: false,
    notable: true,
    lines: true,
    languages: true,
  }
) %>