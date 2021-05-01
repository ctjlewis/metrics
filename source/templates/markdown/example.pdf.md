## Open Source Resume
Powered by [lowlighter/metrics](https://github.com/lowlighter/metrics)

<%- await embed(
  `resume-header`, 
  {
    base: ['header'],
  }
) %>

<%- await include(`partials/rss.ejs`) %>

## Basic info
<%- await embed(
  `resume-basic-info`, 
  {
    isocalendar: true,
    isocalendar_duration: 'full-year',
    base: ['activity', 'community', 'repositories', 'metadata'],
    stackoverflow: true,
    stackoverflow_sections: ['answers-top', 'answers-recent'],
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