def knit_scarf(length, width, pattern='plain'):
    for i in range(length):
        row = ''
        for j in range(width):
            if pattern == 'plain':
                row += 'K'  # Knit stitch
            elif pattern == 'rib':
                if j % 2 == 0:
                    row += 'K'  # Knit stitch
                else:
                    row += 'P'  # Purl stitch
            elif pattern == 'cable':
                if j % 10 == 0:
                    row += 'C'  # Cable stitch
                else:
                    row += 'K'  # Knit stitch
        print(row)

# Example usage
if __name__ == "__main__":
    print("Plain Scarf:")
    knit_scarf(length=10, width=20, pattern='plain')

    print("\nRibbed Scarf:")
    knit_scarf(length=10, width=20, pattern='rib')

    print("\nCable Scarf:")
    knit_scarf(length=10, width=20, pattern='cable')
# XXX-
