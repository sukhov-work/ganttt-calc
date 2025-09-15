# Team Gantt Board

A powerful, browser-based Gantt chart tool for agile team planning and resource management. Built with pure HTML/JavaScript, requiring no backend or external dependencies.

## 🎯 Overview

This tool solves the complexity of managing team capacity and task allocation across quarters. Unlike traditional spreadsheet-based planning, it provides visual drag-and-drop functionality with automatic budget tracking and capacity validation.

### Key Problems Solved
- **Capacity Planning**: Visualize team member availability and workload distribution
- **Budget Tracking**: Ensure task allocations match planned budgets
- **Flexible Scheduling**: Easily redistribute work without breaking totals
- **Fractional Allocation**: Support for partial time allocation (e.g., 50% for team leads)
- **Multi-person Tasks**: Split single features across multiple team members

## ✨ Features

### Core Functionality
- **Drag & Drop Interface**: Intuitive task placement and rearrangement
- **Two Planning Modes**:
    - **Granular Mode**: Drag individual week blocks for maximum flexibility
    - **Continuous Mode**: Drag entire task durations as single blocks
- **Smart Stacking**: Multiple tasks in the same week automatically split capacity
- **Real-time Budget Validation**: Instant feedback on over/under allocations
- **Undo/Redo**: Full history tracking with 50-state buffer
- **Auto-save**: Continuous saving to browser localStorage

### Task Management
- **Task Templates**: Define reusable tasks with duration and color coding
- **Adjustable Duration**: Modify task lengths without recreation
- **Resize on Board**: Drag block edges to extend/reduce duration
- **Week-by-Week Splitting**: Distribute single features across team and time
- **Visual Highlighting**: Hover over templates to see all placements

### Team Management
- **Dynamic Team Size**: Add/remove team members on the fly
- **Quarterly Planning**: 13-week quarters (standard business quarters)
- **Capacity Tracking**: Per-person and total utilization percentages
- **Special Allocations**:
    - Jump weeks (random production tasks)
    - TL Buffer (50% capacity for team leads)

### Data Persistence
- **Browser Storage**: Auto-saves after every change
- **File Export/Import**: Save projects as JSON files
- **Complete State Preservation**: Includes undo history

## 🚀 Getting Started

### Installation
1. Download the HTML file
2. Open in any modern web browser
3. Start planning!

No installation, dependencies, or server required.

### Quick Start Guide

#### 1. Set Up Your Team
- Click "Add Person" to add team members
- Name format: Use "TL" or "Lead" in names for team lead features

#### 2. Create Task Templates
- Click "Add Task Template"
- Enter task name, duration (weeks), and category
- Choose a color for visual organization

#### 3. Assign Tasks

**Granular Mode (Default)**:
- Each template shows individual week blocks (W1, W2, W3...)
- Drag specific weeks to different people/times
- Perfect for splitting features across the team

**Continuous Mode**:
- Templates appear as solid blocks
- Drag entire durations at once
- Ideal for uninterrupted work assignments

#### 4. Manage Allocations
- **Stack Tasks**: Drop multiple tasks on the same week - capacity auto-splits
- **Resize**: Hover over blocks to see resize handle on the right
- **Remove**: Double-click any block to delete
- **Move**: Drag blocks to new positions

#### 5. Monitor Budget
The Summary panel shows three key metrics:
- **Person Utilization**: Individual capacity usage
- **Task Allocation**: Actual vs. planned weeks per task
- **Total Capacity**: Overall team utilization

Status indicators:
- ✓ = Budget matched
- ⚠️ Under = Not fully allocated
- ⚠️ Over = Exceeded budget

## 📊 Use Cases

### Sprint Planning
Plan 2-week sprints with granular task distribution across the team.

### Quarterly Roadmapping
Visualize entire quarter (13 weeks) with major features and dependencies.

### Resource Balancing
Identify over/under-utilized team members and redistribute work.

### Capacity Planning
Account for vacations, part-time work, and administrative overhead.

## 💡 Tips & Best Practices

1. **Start with Templates**: Define all major features as templates before assigning
2. **Use Colors**: Group related tasks by color (e.g., blue for development, green for design)
3. **Regular Saves**: While auto-save is active, use "Save Project" for important milestones
4. **Fractional Planning**: Stack multiple small tasks in the same week for realistic planning
5. **Buffer Time**: Use TL Buffer or Jump weeks for unplanned work

## 🔧 Advanced Features

### Fractional Capacity
When multiple tasks occupy the same person-week:
- Each task gets equal fraction of that week
- Example: 3 tasks in one week = 0.33w each
- Summary accurately reflects fractional allocations

### Task Dependencies
Visual dependency arrows show task relationships (placeholder for future enhancement).

### Optimize Function
"Optimize Gantt" button ready for custom optimization algorithms.

## 🗂️ Data Management

### Auto-save
- Every change automatically saves to browser localStorage
- Persists through browser restarts
- Visual confirmation: "✓ Auto-saved"

### Manual Save/Load
- **Save to Browser**: Explicit save with visual feedback
- **Load from Browser**: Restore previous session
- **Save Project**: Export as JSON file
- **Load Project**: Import from JSON file

### Clear Board
Removes all assignments while preserving templates and team members.

## ⚙️ Technical Details

- **Technology**: Pure HTML5, CSS3, JavaScript (ES6+)
- **Storage**: LocalStorage API for persistence
- **Compatibility**: All modern browsers (Chrome, Firefox, Safari, Edge)
- **Performance**: Handles 10+ team members, 100+ assignments efficiently
- **File Format**: JSON for easy integration and version control

## 🐛 Known Limitations

1. **Browser Storage Limit**: ~5-10MB depending on browser
2. **No Multi-user Sync**: Single-user tool (consider version control for collaboration)
3. **No Backend**: All data stored locally in browser

## 🚦 Roadmap

Future enhancements under consideration:
- [ ] Task dependencies with constraint checking
- [ ] Smart optimization algorithm
- [ ] Export to Excel/CSV
- [ ] Custom week ranges
- [ ] Resource types beyond people
- [ ] Integration with project management tools

## 📝 License

Open source - feel free to modify and adapt for your team's needs.

## 🤝 Contributing

Contributions welcome! The codebase is self-contained in a single HTML file for easy modification.

### Development Guidelines
1. Maintain single-file structure
2. Preserve auto-save functionality
3. Test undo/redo after changes
4. Ensure localStorage compatibility

## 📧 Support

For issues, feature requests, or questions, please open an issue in the repository.

---

*Built to replace complex spreadsheet-based planning with an intuitive, visual approach to team capacity management.*