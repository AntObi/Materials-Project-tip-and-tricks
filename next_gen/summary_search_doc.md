
        Query core data using a variety of search criteria.

        Arguments:
            band_gap (Tuple[float,float]): Minimum and maximum band gap in eV to consider.
            chemsys (str, List[str]): A chemical system, list of chemical systems
                (e.g., Li-Fe-O, Si-*, [Si-O, Li-Fe-P]), or single formula (e.g., Fe2O3, Si*).
            crystal_system (CrystalSystem): Crystal system of material.
            density (Tuple[float,float]): Minimum and maximum density to consider.
            deprecated (bool): Whether the material is tagged as deprecated.
            e_electronic (Tuple[float,float]): Minimum and maximum electronic dielectric constant to consider.
            e_ionic (Tuple[float,float]): Minimum and maximum ionic dielectric constant to consider.
            e_total (Tuple[float,float]): Minimum and maximum total dielectric constant to consider.
            efermi (Tuple[float,float]): Minimum and maximum fermi energy in eV to consider.
            elastic_anisotropy (Tuple[float,float]): Minimum and maximum value to consider for the elastic anisotropy.
            elements (List[str]): A list of elements.
            energy_above_hull (Tuple[int,int]): Minimum and maximum energy above the hull in eV/atom to consider.
            equilibrium_reaction_energy (Tuple[float,float]): Minimum and maximum equilibrium reaction energy in
                eV/atom to consider.
            exclude_elements (List(str)): List of elements to exclude.
            formation_energy (Tuple[int,int]): Minimum and maximum formation energy in eV/atom to consider.
            formula (str, List[str]): A formula including anonymized formula
                or wild cards (e.g., Fe2O3, ABO3, Si*). A list of chemical formulas can also be passed
                (e.g., [Fe2O3, ABO3]).
            g_reuss (Tuple[float,float]): Minimum and maximum value in GPa to consider for the Reuss average
                of the shear modulus.
            g_voigt (Tuple[float,float]): Minimum and maximum value in GPa to consider for the Voigt average
                of the shear modulus.
            g_vrh (Tuple[float,float]): Minimum and maximum value in GPa to consider for the Voigt-Reuss-Hill
                average of the shear modulus.
            has_props: (List[HasProps]): The calculated properties available for the material.
            has_reconstructed (bool): Whether the entry has any reconstructed surfaces.
            is_gap_direct (bool): Whether the material has a direct band gap.
            is_metal (bool): Whether the material is considered a metal.
            k_reuss (Tuple[float,float]): Minimum and maximum value in GPa to consider for the Reuss average
                of the bulk modulus.
            k_voigt (Tuple[float,float]): Minimum and maximum value in GPa to consider for the Voigt average
                of the bulk modulus.
            k_vrh (Tuple[float,float]): Minimum and maximum value in GPa to consider for the Voigt-Reuss-Hill
                average of the bulk modulus.
            magnetic_ordering (Ordering): Magnetic ordering of the material.
            material_ids (List[MPID]): List of Materials Project IDs to return data for.
            n (Tuple[float,float]): Minimum and maximum refractive index to consider.
            num_elements (Tuple[int,int]): Minimum and maximum number of elements to consider.
            num_sites (Tuple[int,int]): Minimum and maximum number of sites to consider.
            num_magnetic_sites (Tuple[int,int]): Minimum and maximum number of magnetic sites to consider.
            num_unique_magnetic_sites (Tuple[int,int]): Minimum and maximum number of unique magnetic sites to consider.
            piezoelectric_modulus (Tuple[float,float]): Minimum and maximum piezoelectric modulus to consider.
            poisson_ratio (Tuple[float,float]): Minimum and maximum value to consider for Poisson's ratio.
            possible_species (List(str)): List of element symbols appended with oxidation states. (e.g. Cr2+,O2-)
            shape_factor (Tuple[float,float]): Minimum and maximum shape factor values to consider.
            spacegroup_number (int): Space group number of material.
            spacegroup_symbol (str): Space group symbol of the material in international short symbol notation.
            surface_energy_anisotropy (Tuple[float,float]): Minimum and maximum surface energy anisotropy values
                to consider.
            theoretical: (bool): Whether the material is theoretical.
            total_energy (Tuple[int,int]): Minimum and maximum corrected total energy in eV/atom to consider.
            total_magnetization (Tuple[float,float]): Minimum and maximum total magnetization values to consider.
            total_magnetization_normalized_formula_units (Tuple[float,float]): Minimum and maximum total magnetization
                values normalized by formula units to consider.
            total_magnetization_normalized_vol (Tuple[float,float]): Minimum and maximum total magnetization values
                normalized by volume to consider.
            uncorrected_energy (Tuple[int,int]): Minimum and maximum uncorrected total energy in eV/atom to consider.
            volume (Tuple[float,float]): Minimum and maximum volume to consider.
            weighted_surface_energy (Tuple[float,float]): Minimum and maximum weighted surface energy
                in J/m² to consider.
            weighted_work_function (Tuple[float,float]): Minimum and maximum weighted work function in eV to consider.
            sort_fields (List[str]): Fields used to sort results. Prefixing with '-' will sort in descending order.
            num_chunks (int): Maximum number of chunks of data to yield. None will yield all possible.
            chunk_size (int): Number of data entries per chunk.
            all_fields (bool): Whether to return all fields in the document. Defaults to True.
            fields (List[str]): List of fields in SearchDoc to return data for.
                Default is material_id if all_fields is False.

        Returns:
            ([SummaryDoc]) List of SummaryDoc documents
        