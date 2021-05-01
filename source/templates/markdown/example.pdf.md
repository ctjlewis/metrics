## Open Source Resume
*Generated with [GitHub Metrics](https://github.com/lowlighter/metrics)*

<%- await include(`partials/rss.ejs`) %> 

<%- await embed(
  `resume-header`, 
  {
    base: ['header'],
  }
) %>


### Basic info
<%- await embed(
  `resume-basic-info`, 
  {
    base: ['activity', 'community', 'repositories', 'metadata'],

    repositories_forks: true,
    notable: true,
    lines: true,

    followup: true,
    followup_sections: ['user'],

    languages: true,
    languages_details: ['bytes-size', 'percentage'],
    
    // isocalendar: true,
    // isocalendar_duration: 'full-year',
  }
) %>

<div style="page-break-after: always;"></div>

### Contributions: GitHub
<%- await embed(
  `resume-activity`, 
  {
    base: [],

    activity: true,
    activity_days: 0,
    activity_limit: 15,
    activity_filter: [
      'issue',
      'pr'
    ],
  }
) %>

<div style="page-break-after: always;"></div>

### Contributions: StackOverflow
<%- await embed(
  `resume-stackoverflow`,
  {
    base: [],

    stackoverflow: true,
    stackoverflow_sections: ['answers-top', 'answers-recent'],
    stackoverflow_user: 1674992,
    stackoverflow_limit: 2,
    stackoverflow_lines: 8,
  }
) %>
