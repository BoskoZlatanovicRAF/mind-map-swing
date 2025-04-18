# Gerumap - Mind Mapping Software

## Overview
Gerumap is a Java-based desktop application for creating, editing, and visualizing mind maps. The application allows users to create organized visual representations of their ideas and concepts with an intuitive graphical interface.

## Technologies Used
- **Java** - Core programming language
- **Swing** - For building the graphical user interface
- **Maven** - Dependency management
- **Lombok** - To reduce boilerplate code
- **Gson** - JSON serialization/deserialization for saving and loading projects

## Key Features

### Project Management
- Create and manage multiple mind mapping projects
- Organize mind maps within projects
- Add author information to projects
- Save, load, and export functionality

### Mind Map Editing
- Create concept nodes with customizable properties
- Connect concepts with relationship lines
- Add a main concept as the central node of your mind map
- Move, resize, and delete elements
- Customize colors and stroke weights

### Advanced Visualization Features
- Zoom in/out functionality
- Move/pan the canvas
- "Best Fit" automatic layout reorganization
- Select multiple elements for bulk operations
- Export mind maps as images

### State-Based Interaction
- Different interaction states for various editing operations
- Selection, creation, deletion, and movement states
- Intuitive state switching through toolbar buttons

### Command Pattern Implementation
- Undo/redo functionality for all operations
- Command history tracking

## Architecture
The application follows several design patterns:
- **Composite Pattern** - For the hierarchical structure of projects and mind maps
- **Observer Pattern** - For updating views when model changes
- **Factory Pattern** - For creating different types of nodes
- **Command Pattern** - For undo/redo functionality
- **State Pattern** - For different interaction modes
- **Singleton Pattern** - For managing application core components

## Getting Started
1. Clone the repository
2. Build the project using Maven: `mvn clean install`
3. Run the application
4. Create a new project using the "New Project" button
5. Create mind maps within your project
6. Save your work using the "Save" button

## Project Structure
- The application follows MVC architecture
- GUI components are in the `gui.swing` package
- Core interfaces and implementations are in the `core` package
- Mind map structure and operations are in the `mapRepository` package
- Error handling and logging in the `errorHandling` package
- Serialization utilities in the `serializable` package
