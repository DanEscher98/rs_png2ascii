# Development plan

## Month 1
1. Set up the project structure and initialize a new Rust project.
2. Add necessary dependencies to the project, including the image crate for PNG
   decoding and the colored crate for terminal coloring.
3. Implement the PNG decoding functionality using the image crate to read and
   parse the PNG file.
4. Write a function to convert each pixel of the PNG image to its corresponding
ASCII character based on brightness or color intensity.
    - Use the ASCII character mapping based on brightness levels.
    - Extract the color information for each pixel to be used for color mapping
      later.

## Month 2
1. Implement the ASCII character mapping based on color.
    - Map the color values extracted from the original image to the closest
      matching ASCII color using predefined color values in the colored crate.
    - Apply the corresponding color to the ASCII character in the output.
2. Write a function to generate the ASCII art string by iterating over each
pixel of the image and mapping it to the ASCII character and color.
3. Test the ASCII generation functionality with different PNG images, ensuring
the accuracy of the ASCII representation and color mapping.


## Month 3
1. Add command-line interface (CLI) functionality using `clap`
    - Define the command-line arguments and options to specify the input PNG
      file, output file or printing to the terminal, color or grayscale mode,
      etc.
    - Parse the command-line arguments and options to drive the generation of
      the ASCII art.
2. Implement file saving functionality to allow the user to save the generated
ASCII art to a text file.
3. Perform comprehensive testing and debugging to ensure the stability and
reliability of the CLI tool.
4. Document the code, write unit tests, and follow best practices for Rust
development.
