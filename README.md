# phaseone
Road to OMSCS

Phase One will consist of a series of projects to help me prepare for my journey into the OMSCS degree with an AI specialization. 
Project One: 
  Virtual Environments:
  Project completed: The Dual-Environment Dependency Challenge

To demonstrate your proficiency in managing isolated Python environments, you will simulate a common scenario encountered in OMSCS coursework: balancing multiple projects with conflicting library requirements.

Your Assignment:

Initialize Two Projects: Create two distinct project directories on your local machine. Name them Project_Alpha and Project_Beta.

Establish Isolation: Create a separate virtual environment for each project using either venv or conda.

Induce a Version Conflict: * In the Project_Alpha environment, install the numpy library strictly locked to version 1.21.0.

In the Project_Beta environment, install the numpy library strictly locked to version 2.4.0 (Changed version number due to ignored yanks).

Generate Manifests: Extract the exact state of each environment by generating a dependency manifest (e.g., a requirements.txt file) within their respective project folders.

Verify Reproducibility: * Completely deactivate all environments.

Create a third, entirely new environment called Project_Gamma.

Using only the manifest file you generated from Project_Alpha, perfectly recreate Project_Alpha's environment state inside Project_Gamma.

Success Criteria: You have successfully completed this task when you can activate Project_Alpha and Project_Beta back-to-back, programmatically print the installed numpy version from the command line in each, and see two different version numbers without any system-wide conflicts. Furthermore, inspecting the Project_Gamma manifest should yield an exact match to Project_Alpha.
