# Images Directory Structure

This directory contains all images used in the One Flow Operating Playbook documentation.

## 📁 Folder Organization

### `/sops/` - SOP-Specific Images
Images that are specific to individual Standard Operating Procedures.

- **`ambassador-program/`** - Ambassador Program SOP images
  - Flow Groups structure diagrams
  - Ambassador application screenshots
  - Event planning templates
  - Drops compensation tracking examples

- **`move-in-sop/`** - Move-In SOP images
  - Move-in checklist examples
  - Welcome gift setup photos
  - Unit walkthrough guides
  - Carson access setup screenshots

- **`neighbor-communication/`** - Neighbor Communication SOP images
  - Email template examples
  - Communication flow diagrams
  - Channel-specific screenshots

- **`unit-readiness/`** - Unit Move-In Readiness SOP images
  - Unit inspection checklists
  - Maintenance completion photos
  - Readiness verification screenshots

### `/systems/` - System Screenshots & Diagrams
Screenshots and diagrams of Flow's technology stack.

- **`yardi/`** - Yardi Voyager screenshots
  - Dashboard views
  - Resident profiles
  - Workflow interfaces
  - Report examples

- **`carson/`** - Carson/Flow App screenshots
  - Access control interfaces
  - Delivery notifications
  - Amenity booking screens

- **`moved/`** - Moved platform screenshots
  - Move-in checklists
  - Progress tracking
  - Completion status views

- **`zendesk/`** - Zendesk support screenshots
  - Ticket management
  - Communication templates
  - Escalation workflows

### `/workflows/` - Process Flow Diagrams
Visual representations of processes and workflows.

- Process flowcharts
- Decision trees
- Integration diagrams
- Handoff sequences

### `/templates/` - Template Examples
Example documents and forms.

- SOP template examples
- Checklist templates
- Communication templates
- Report formats

### `/icons/` - Icons and Small Graphics
Icons, logos, and small graphical elements.

- System icons
- Status indicators
- Navigation elements
- Decorative graphics

## 📝 Naming Conventions

### File Naming
- Use descriptive names: `yardi-voyager-dashboard.png`
- Use hyphens, not spaces: `move-in-checklist-example.png`
- Include version numbers if needed: `ambassador-application-v2.png`
- Use lowercase letters

### Folder Naming
- Use lowercase with hyphens: `ambassador-program/`
- Keep names concise but descriptive
- Match SOP names when possible

## 🖼️ Image Guidelines

### File Formats
- **Screenshots**: PNG for clarity and text readability
- **Diagrams**: SVG for scalability and crisp rendering
- **Photos**: JPG for smaller file sizes
- **Icons**: SVG or PNG (SVG preferred for scalability)

### Size Guidelines
- **Screenshots**: Maximum 1200px width
- **Diagrams**: SVG preferred for scalability
- **Thumbnails**: 300-400px width
- **Icons**: 16px, 24px, 32px, 48px, 64px standard sizes

### Quality Standards
- High resolution for screenshots
- Clear, readable text in images
- Consistent styling across similar images
- Optimized file sizes for web performance

## 🔗 Referencing Images in Markdown

### Relative Paths
```markdown
![Image Description](../images/sops/ambassador-program/flow-groups-structure.png)
![Yardi Dashboard](../images/systems/yardi/voyager-dashboard.png)
```

### Alt Text
Always include descriptive alt text for accessibility:
```markdown
![Yardi Voyager resident profile interface showing personal information and lease details](../images/systems/yardi/resident-profile.png)
```

## 📋 Usage Examples

### SOP Images
```markdown
## Screenshots & Visuals
- [Placeholder: Moved - Unit Readiness Checklist view](../images/sops/unit-readiness/moved-checklist.png)
- [Placeholder: Carson - Access system testing screen](../images/systems/carson/access-testing.png)
```

### System Documentation
```markdown
![Yardi Voyager Workflow Dashboard showing pending approvals](../images/systems/yardi/workflow-dashboard.png)
```

## 🚀 Adding New Images

1. **Choose the appropriate folder** based on content type
2. **Use descriptive naming** following conventions
3. **Optimize file size** for web performance
4. **Update this README** if adding new folder categories
5. **Reference in documentation** using relative paths

## 📞 Support

For questions about image organization or usage, contact the documentation team or refer to the main playbook guidelines.
