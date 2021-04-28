# GitHub Resume
### Powered by [lowlighter/metrics](https://github.com/lowlighter/metrics)

<%- await include(`partials/rss.ejs`) %>

# Basic info
<%- await embed(
  `base`, 
  {
    base: ['activity', 'community', 'repositories', 'metadata']
  }
) %>

<%- await embed(
  `calendar`, 
  {
    isocalendar: true
  }
) %>
