<%- await include(`partials/rss.ejs`) %> 

<%- await embed(
  `resume-header`, 
  {
    base: ['header'],
  }
) %>

<div style="padding-top: 2vh;"></div>

*Generated with [GitHub Metrics](https://github.com/lowlighter/metrics).*

#### Summary: GitHub
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

<div style="break-after: always; page-break-after: always;"></div>
<div style="padding-top: 3vh;"></div>

#### Contributions: GitHub
<%- await embed(
  `resume-activity`, 
  {
    base: [],

    activity: true,
    // activity_days: 180,
    // activity_limit: 50,
    activity_filter: [
      'issue',
      'pr'
    ],
  }
) %>

<div style="break-after: always; page-break-after: always;"></div>
<div style="padding-top: 3vh;"></div>

#### Contributions: StackOverflow
<%- await embed(
  `resume-stackoverflow`,
  {
    base: [],

    stackoverflow: true,
    stackoverflow_sections: ['answers-recent'],
    stackoverflow_user: 1674992,
    stackoverflow_limit: 5,
    stackoverflow_lines: 4,
  }
) %>
