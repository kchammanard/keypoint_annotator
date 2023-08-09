# CVAT to COCO (YOLOv8) Converter

## Annotation Instructions

1. Visit [cvat.ai](https://cvat.ai) and create an account.
2. Create a new project and define a label (any name will suffice).
3. Configure the label as a "point" in the project settings.
4. Create a task and import your dataset.
5. Annotate keypoints by placing points on the images. Press 'N' after each point placement to save and add another point.
6. If a point is obscured or not visible, hover over it and press "Q" to mark it as "Occluded".
7. Once all images are annotated, export the annotations as "CVAT for images 1.1".

## CVAT to COCO Instructions

1. Import the previously generated annotations file and name it "annotations.xml".
2. Place the "annotations.xml" file in the root directory of your project.
3. Run the "cvat_to_coco.py" script.
4. The resulting COCO-formatted annotations will be available in the "out" folder.

## File Format

Each annotation file adheres to the following format:
<br>
`index (default 0), x_centroid, y_centroid, width, height, x1, y1, v1, x2, y2, v2, ...`

For more detailed instructions, you can refer to this [tutorial video](https://www.youtube.com/watch?v=gA5N54IO1ko).
