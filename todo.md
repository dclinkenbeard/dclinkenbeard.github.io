# Jekyll Blog Customization Plan

This document outlines the steps needed to customize your Jekyll al-folio blog with your personal information, social media links, and professional details.

## 1. Social Media and Contact Information (`_data/socials.yml`)

**Current Status**: Only email is configured (dclinkenbeard@csumb.edu)

**Actions Needed**:

- [x] Add GitHub username
- [x] Add LinkedIn profile
- [ ] ~Add Twitter/X handle (if applicable)~
- [x] Add Google Scholar ID
- [x] Add ORCID ID (for academic publications)
- [ ] Add any other relevant social platforms:
  - ResearchGate profile
  - Academia.edu profile
  - Personal website/portfolio
  - Professional blog
  - YouTube channel (if applicable)
  - Mastodon/Bluesky (if applicable)

## 2. Main Configuration (`_config.yml`)

**Current Status**: Basic info configured, needs review and updates

**Actions Needed**:

- [ ] Verify and update site title if needed
- [ ] Review and update site description
- [ ] Update footer text with personal preferences
- [ ] Review keywords for SEO optimization
- [ ] Verify URL (currently set to clinkenbeard.info)
- [ ] Update favicon if desired
- [ ] Review theme settings (light/dark modes)

## 3. About Page (`_pages/about.md`)

**Current Status**: Basic template with placeholder content

**Actions Needed**:

- [ ] Update subtitle with actual affiliations
- [ ] Replace profile image with your professional photo
- [ ] Update contact information and office details
- [ ] Write comprehensive bio content
- [ ] Configure selected papers display
- [ ] Set up announcements/news section
- [ ] Configure latest posts display preferences

## 4. CV Data (`_data/cv.yml`)

**Current Status**: Partially filled with basic information

**Actions Needed**:

- [ ] Complete education section descriptions
- [ ] Expand experience section with detailed descriptions
- [ ] Add publications section
- [ ] Add skills/technical competencies
- [ ] Add awards and honors
- [ ] Add professional memberships
- [ ] Add conferences and presentations
- [ ] Add teaching experience details
- [ ] Add research interests
- [ ] Add service and committee work

## 5. Profile Assets

**Actions Needed**:

- [ ] Add professional profile photo to `assets/img/`
- [ ] Optimize image for web (Jekyll will handle responsive formats)
- [ ] Update any other imagery used throughout the site

## 6. Additional Data Files

**Review and Update**:

- [ ] `_data/repositories.yml` - GitHub repositories to showcase
- [ ] `_data/coauthors.yml` - Research collaborators
- [ ] `_data/venues.yml` - Publication venues

## 7. Content Creation

**Actions Needed**:

- [ ] Create initial blog posts in `_posts/`
- [ ] Set up projects in `_projects/`
- [ ] Configure publications (if using Jekyll Scholar)
- [ ] Create any additional pages needed

## 8. SEO and Analytics

**Actions Needed**:

- [ ] Set up Google Analytics (if desired)
- [ ] Configure SEO tags and meta descriptions
- [ ] Set up site verification for search engines
- [ ] Configure RSS feed settings

## 9. Theme Customization

**Optional Enhancements**:

- [ ] Customize color scheme in `_sass/`
- [ ] Adjust layout preferences
- [ ] Configure commenting system (if desired)
- [ ] Set up search functionality
- [ ] Configure dark/light mode preferences

## 10. Final Testing and Deployment

**Actions Needed**:

- [ ] Test site locally with `bundle exec jekyll serve --livereload`
- [ ] Verify all links work correctly
- [ ] Test responsive design on mobile devices
- [ ] Check site performance and loading times
- [ ] Run final formatting with Prettier
- [ ] Deploy to GitHub Pages

## Priority Order

1. **High Priority**: Social media links, About page content, CV data
2. **Medium Priority**: Profile photo, additional content creation
3. **Low Priority**: Theme customization, advanced features

## Notes

- All changes should be tested locally before pushing to production
- Keep backups of original files before making major changes
- Follow Jekyll and al-folio documentation for advanced customizations
- Consider SEO best practices when writing content
- Maintain academic/professional tone appropriate for your field

## Questions to Consider

Before starting customization, consider:

- Which social media platforms are most relevant for your professional presence?
- What sections of your CV should be prominently featured?
- What type of content do you want to regularly publish (blog posts, research updates, etc.)?
- Do you want to enable comments on your blog posts?
- What's your preference for the overall design aesthetic?
